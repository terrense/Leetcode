
**LeetCode Solutions by Problem Number（C++ 实现，后续不断更新）**



---

```md
# 📘 LeetCode Solutions (C++ by Problem Number)

---

## 🌍 English

Welcome to my **LeetCode Solutions** repository.  
Here I solve problems **by their official number** (e.g., `0001 Two Sum`, `0002 Add Two Numbers`) using **modern C++ (C++17/20)**.  

📌 Goals:
- Build a structured archive of solutions (indexed by LeetCode problem number).  
- Improve **algorithmic thinking** and **C++ coding skills**.  
- Provide clean, well-commented, and efficient code.  

📂 Repository Structure:
```

├── 0001\_two\_sum.cpp
├── 0002\_add\_two\_numbers.cpp
├── 0003\_longest\_substring.cpp
...

```

💡 Each file contains:
- Problem statement (short summary)  
- My C++ solution  
- Explanation / comments  

🚀 Updates will come as I solve more problems!

---

## 🌍 Русский

Добро пожаловать в мой репозиторий **LeetCode Solutions**.  
Здесь я решаю задачи **по их официальному номеру** (например, `0001 Two Sum`, `0002 Add Two Numbers`) на **современном C++ (C++17/20)**.  

📌 Цели:
- Построить структурированный архив решений (индексированных по номеру задачи).  
- Прокачать **алгоритмическое мышление** и навыки программирования на **C++**.  
- Давать чистый, хорошо прокомментированный и эффективный код.  

📂 Структура репозитория:
```

├── 0001\_two\_sum.cpp
├── 0002\_add\_two\_numbers.cpp
├── 0003\_longest\_substring.cpp
...

```

💡 Каждый файл содержит:
- Краткое условие задачи  
- Решение на C++  
- Объяснения / комментарии  

🚀 Репозиторий будет обновляться по мере решения новых задач!

---

## 🌍 中文

欢迎来到我的 **LeetCode 题解仓库**。  
我会按照 **题目编号顺序**（如 `0001 两数之和`, `0002 两数相加`）用 **现代 C++ (C++17/20)** 编写题解。  

📌 目标：
- 建立一个 **按题号索引的题解归档**  
- 提升 **算法思维** 和 **C++ 编程能力**  
- 提供 **简洁、高效、注释清晰** 的代码  

📂 仓库结构：
```

├── 0001\_two\_sum.cpp
├── 0002\_add\_two\_numbers.cpp
├── 0003\_longest\_substring.cpp
...

````

💡 每个文件包含：
- 题目简述  
- 我的 C++ 代码实现  
- 注释 / 解释  

🚀 仓库会持续更新！

---

## ⚡ Example Solution (C++)

**0001 Two Sum**

```cpp
#include <bits/stdc++.h>
using namespace std;

class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        unordered_map<int, int> mp; // value -> index
        for (int i = 0; i < nums.size(); i++) {
            int need = target - nums[i];
            if (mp.count(need)) {
                return {mp[need], i};
            }
            mp[nums[i]] = i;
        }
        return {};
    }
};

int main() {
    Solution s;
    vector<int> nums = {2, 7, 11, 15};
    int target = 9;
    auto res = s.twoSum(nums, target);
    cout << res[0] << " " << res[1] << endl; // Output: 0 1
}
````

---

📌 Stay tuned — I will keep adding solutions regularly!

```

