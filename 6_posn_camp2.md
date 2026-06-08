[<- หน้าก่อนหน้า](5_posn_camp1.md) | [หน้าต่อไป ->](7_toi.md)
---

# 6. สอวน ค่าย 2

## 6.1 รายละเอียดการจัดค่าย

ตัวค่ายจะจัดช่วง ปิดเทอม 2 (เริ่ม ต้น-กลางเดือนมีนาคม)

## 6.2 การคัดเด็กไปค่ายต่อไป

คัดจาก 30 คน + คนสอบท้ายค่าย 2 -> ผู้แทนศูนย์ 5 คน

## 6.3 สิทธิ์พิเศษกรณีสอบไม่ผ่านค่าย

มีสิทธิ์วนสอวน ค่าย 2

## 6.4 เนื้อหา

เนื้อหาในค่าย 2 นั้นน้องๆจะต้องเขียนโปรแกรมที่เร็วและใช้ memory น้อยซึ่งต่างจากค่าย 1 ที่จะเขียนยังไงก็ได้

### 6.4.1 เนื้อหาที่สอน (เนื้อหาตั้งแต่ค่าย 2 ขึ้นไปจะค่อนข้างซ้ำๆกันเพราะงั้นควรเรียนทุกเรื่องให้เข้าใจ)

ทั้งนี้จากประสบการณ์ของพี่ ค่าย สอวน จะสอนเนื้อหาไม่ค่อยครบและมันสามารถออกอะไรก็ได้ แต่ก็มีเนื้อหาที่อยู่ในตารางจะมีดังนี้

- Data structure (C++ STL / Heap(Priority queue))
- BFS / DFS / Recursion
- Dynamic programming
- Binary search
- Divide and Conquer
- Graph : Traversal (Ex: Checking Is graph is bipartite)
- Graph : Shortest path / Minimum spanning tree

ในส่วนนี้จะเป็นเนื้อหาที่มีโอกาสออกแต่ไม่ได้สอน
- Prefix sum
- Sliding Window
- Two pointer
- Constructive algorithm
- โจทย์แนวไหวพริบ หรือ Observation (โจทย์ที่ต้องอาศัยไหวพริบเป็นหลัก อาจจะประยุกต์กับ Data structure บ้าง)

### 6.4.1.1 Ranking ตาม โอกาสในการออกสอบ (เฉพาะที่สอนในค่าย)
1. Graph : Shortest path
2. Dynamic programming
3. Data Structure (C++ STL)
4. Graph : Minimum spanning tree
5. Binary search
6. BFS DFS Recursion
7. Greedy
8. Divide and Conquer (ปกติจะไม่ค่อยออกเพราะเป็นเนื้อหาที่ค่อนข้างเป็นการจำ Algorithm หรือถ้าไม่จำก็จะยากไปเลย)

### 6.4.1.2 ขยายเพิ่มเติมเกี่ยวกับ Data structure
ส่วนตัวพี่คงคิดว่าหลายคนคงสับสนว่า Data structure มันจะออกยังไงเพราะว่าในการเขียนโปรแกรมปกติมันก็ต้องใช้ Data structure อยู่แล้ว แต่ในความเป็นจริงเราสามารถประยุกต์ Data structure ได้ดังนี้

- **ถ้าโจทย์บีบเรื่อง Memory**: สมมติโจทย์ให้เลขถึง 1e9 การประกาศ array ใหญ่ๆ แบบปกติมันจะโดน Memory เกิน (MLE) เราเลยต้องหันมาใช้ map หรือ unordered_map เพื่อเก็บแค่ค่าที่เราใช้จริงๆ แทน
- **ถ้าโจทย์บีบเรื่องความเร็ว**: อย่างโจทย์ [Trapping Rain Water บน LeetCode](https://leetcode.com/problems/trapping-rain-water/description/) ถ้าเราเขียน Brute-force เช็คทุกจุดอาจต้องใช้ O(n²) ซึ่งช้าจนเกิน Time Limit แต่ถ้าเราใช้ Monotonic Stack มาจัดการข้อมูลให้เป็นระเบียบ เราจะลดมันเหลือแค่ O(n) ได้เลย

### 6.4.1.3 คำแนะนำ ในส่วนของ Divide and Conquer เผื่อคนอยากเตรียมเนื้อหา
แนะนำให้เขียนฝึกเขียน Merge Sort ให้เป็นเพราะหลายๆ algorithm ในเนื้อหานี้จะประยุกต์กับ Merge Sort บ่อย
Ex: [Pair 1109 บน programming.in.th](https://programming.in.th/tasks/1109)

### 6.4.1.4 Algorithm ที่ควรรู้
- [LIS in O(n log n) - GeeksforGeeks](https://www.geeksforgeeks.org/dsa/longest-increasing-subsequence-dp-3/)
- [Finding Prime Number in O(n loglog n) (Sieve of Eratosthenes) - GeeksforGeeks](https://www.geeksforgeeks.org/dsa/sieve-of-eratosthenes/)

## 6.5 เทคนิค

### 6.5.1 การเรียนรู้
- โจทย์ตั้งแต่สอวน. ค่าย 2 ขึ้นไปจะเป็นโจทย์ยากและใช้เวลาในการทำไม่เหมือนกับการสอบเข้าค่าย 1 และค่าย 1 ที่เป็นแนว speed test
- แนะนำให้ลองคิดเองสัก 20–30 นาทีถ้าคิดไม่ออกค่อยดูเฉลย
- ควรแก้บัคด้วยตัวเองก่อน / ฝึกหา Test case เพราะคนส่วนใหญ่จะพลาดที่ Test case ที่เขาให้มาผ่านหมด แต่ส่งไปแล้วได้ 0 คะแนน ถ้าแก้ไม่ได้อาจหาดูของคนอื่นหรือถาม AI ทั้งนี้เราควรรู้ด้วยว่าโปรแกรมเราพลาดตรงไหนไม่ใช่ลบแล้วลอกตามคนอื่นไปเลย
- ถ้าทำโจทย์จบ 1 ข้อแล้วเราไม่รู้สึก improve หรือติดข้อเดิมซ้ำๆแสดงว่าเรากำลังเรียนรู้ผิดวิธี ให้ลองเปลี่ยนวิธีให้เข้ากับตัวเองมากขึ้น
- การถาม AI ในนั้นเป็นสิ่งที่ดีแต่บางครั้ง resource ใน Internet ก็ดีกว่าและแม่นยำกว่า
- ให้ทำ Note ว่าตอนเราฝึกทำโจทย์เราพลาดตรงไหนบ้างเพื่อที่ตอนก่อนเข้าห้องสอบจะได้มาอ่านทำให้เราแก้บัคได้เร็วขึ้น

### 6.5.2 การเขียนโค้ด
- ในหลายสถานการณ์การประกาศตัวแปรให้เป็น constant จะเร็วกว่าเช่นในการ mod ด้วย 1e9+7 ในโจทย์ที่เกี่ยวกับ combination
- การประกาศ vector ไม่ควรใช้ `push_back` เพราะช้ากว่าการประกาศเป็น size เลยเช่น `vector<int>(n)` เนื่องจากแม้จะเป็น O(1) * n ครั้งแต่มี cost แฝงเยอะ อ้างอิงตามบทความ [Amortized Analysis Discussion](https://people.engr.tamu.edu/andreas-klappenecker/csce411-f13/csce411-amortized2.pdf)
- แนะนำให้เรียนวิธีการทำให้โปรแกรมเรา run เร็วขึ้นจาก cache เช่นรูปแบบโค้ดดังนี้

```txt
(1) ช้ากว่าเนื่องจากเข้าถึงข้อมูลแบบกระโดดข้ามแถว (Column-major memory access)
for(int i = 0; i < n; i++) {
    for(int j = 0; j < n; j++) {
        array[j][i]++;
    }
}

(2) เร็วกว่ามากเนื่องจากเข้าถึงข้อมูลเรียงตามแนวหน่วยความจำ (Row-major memory access)
for(int i = 0; i < n; i++) {
    for(int j = 0; j < n; j++) {
        array[i][j]++;
    }
}
