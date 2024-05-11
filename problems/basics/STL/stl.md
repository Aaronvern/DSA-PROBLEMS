### unordered_set in C++ STL:

- **Modifiers:**
  - `insert`
  - `erase`
  - `clear`
- **Capacity:**
  - `empty`
  - `size`
- **Lookup:**
  - `find`
  - `count`
- **Hash Policy:**
  - `load_factor`
  - `max_load_factor`
  - `rehash`
``` 
  #include <iostream>
  #include <unordered_set>

  int main() {
      std::unordered_set<int> mySet;

      // Modifiers
      mySet.insert(1);
      mySet.insert(2);
      mySet.erase(1);
      mySet.clear();

      // Capacity
      bool isEmpty = mySet.empty();
      int size = mySet.size();

      // Lookup
      auto it = mySet.find(2);
      int count = mySet.count(2);

      // Hash Policy
      double loadFactor = mySet.load_factor();
      mySet.max_load_factor(0.5);
      mySet.rehash(100);

      return 0;
  }

```
### vector in C++ STL:

- **Modifiers:**
  - `push_back`
  - `pop_back`
  - `emplace_back`
  - `insert`
  - `erase`
  - `clear`
- **Capacity:**
  - `size`
  - `empty`
  - `reserve`
  - `shrink_to_fit`
- **Element Access:**
  - `operator[]`
  - `at`
  - `front`
  - `back`
- **Iterators:**
  - `begin`
  - `end`
  ``` 
    #include <iostream>
  #include <vector>

  int main() {
      std::vector<int> vec;

      // Modifiers
      vec.push_back(1);
      vec.pop_back();
      vec.emplace_back(2);
      vec.insert(vec.begin() + 1, 3);
      vec.erase(vec.begin());
      vec.clear();

      // Capacity
      int size = vec.size();
      bool isEmpty = vec.empty();
      vec.reserve(100);
      vec.shrink_to_fit();

      // Element Access
      int value = vec[0];
      int value2 = vec.at(0);
      int firstElement = vec.front();
      int lastElement = vec.back();

      // Iterators
      auto it = vec.begin();
      auto endIt = vec.end();

      return 0;
  }

  ```

### set in C++ STL:

- **Modifiers:**
  - `insert`
  - `erase`
  - `clear`
- **Capacity:**
  - `empty`
  - `size`
- **Lookup:**
  - `find`
  - `count`
  - `lower_bound`
  - `upper_bound`
- **Iterators:**
  - `begin`
  - `end`
```
  #include <iostream>
  #include <set>

  int main() {
      std::set<int> mySet;

      // Modifiers
      mySet.insert(1);
      mySet.erase(1);
      mySet.clear();

      // Capacity
      bool isEmpty = mySet.empty();
      int size = mySet.size();

      // Lookup
      auto it = mySet.find(2);
      int count = mySet.count(2);
      auto lb = mySet.lower_bound(2);
      auto ub = mySet.upper_bound(2);

      // Iterators
      auto beginIt = mySet.begin();
      auto endIt = mySet.end();

      return 0;
}

```
### unordered_multiset in C++ STL:

(Functions are similar to unordered_set)
  ``` 
  #include <iostream>
  #include <unordered_set>

  int main() {
      std::unordered_multiset<int> myMultiSet;

      // Functions are similar to unordered_set

      return 0;
  }

  ```
### multiset in C++ STL:

(Functions are similar to set)

``` 
#include <iostream>
#include <set>

int main() {
    std::multiset<int> myMultiSet;

    // Functions are similar to set

    return 0;
}

```

### unordered_map in C++ STL:

- **Modifiers:**
  - `insert`
  - `erase`
  - `clear`
- **Capacity:**
  - `empty`
  - `size`
- **Lookup:**
  - `find`
  - `count`
- **Element Access:**
  - `operator[]`
- **Hash Policy:**
  - `load_factor`
  - `max_load_factor`
  - `rehash`
- **Iterators:**
  - `begin`
  - `end`
  ``` 
  #include <iostream>
  #include <unordered_map>

  int main() {
      std::unordered_map<int, std::string> myMap;

      // Modifiers
      myMap.insert({1, "one"});
      myMap.erase(1);
      myMap.clear();

      // Capacity
      bool isEmpty = myMap.empty();
      int size = myMap.size();

      // Lookup
      auto it = myMap.find(2);
      int count = myMap.count(2);

      // Element Access
      std::string& value = myMap[2];

      // Hash Policy
      double loadFactor = myMap.load_factor();
      myMap.max_load_factor(0.5);
      myMap.rehash(100);

      // Iterators
      auto beginIt = myMap.begin();
      auto endIt = myMap.end();

      return 0;
  }

  ```

### map in C++ STL:

(Functions are similar to unordered_map)
``` 
  #include <iostream>
  #include <map>

  int main() {
      std::map<int, std::string> myMap;

      // Functions are similar to unordered_map

      return 0;
  }

```

### unordered_multimap in C++ STL:

(Functions are similar to unordered_map)
```
  #include <iostream>
  #include <unordered_map>

  int main() {
      std::unordered_multimap<int, std::string> myMultiMap;

      // Functions are similar to unordered_map

      return 0;
  }

```

### queue in C++ STL:

- **Modifiers:**
  - `push`
  - `pop`
- **Capacity:**
  - `empty`
  - `size`
- **Element Access:**
  - `front`
  - `back`
  ``` 
  #include <iostream>
  #include <queue>

  int main() {
      std::queue<int> myQueue;

      // Modifiers
      myQueue.push(1);
      myQueue.pop();

      // Capacity
      bool isEmpty = myQueue.empty();
      int size = myQueue.size();

      // Element Access
      int frontElement = myQueue.front();
      int backElement = myQueue.back();

      return 0;
  }

  ```

### stack in C++ STL:

- **Modifiers:**
  - `push`
  - `pop`
- **Capacity:**
  - `empty`
  - `size`
- **Element Access:**
  - `top`
  ```
  #include <iostream>
  #include <stack>

  int main() {
      std::stack<int> myStack;

      // Modifiers
      myStack.push(1);
      myStack.pop();

      // Capacity
      bool isEmpty = myStack.empty();
      int size = myStack.size();

      // Element Access
      int topElement = myStack.top();

      return 0;
  }

  ```
### deque in C++ STL:

- **Modifiers:**
  - `push_back`
  - `push_front`
  - `pop_back`
  - `pop_front`
  - `emplace_back`
  - `emplace_front`
  - `insert`
  - `erase`
  - `clear`
- **Capacity:**
  - `empty`
  - `size`
- **Element Access:**
  - `operator[]`
  - `at`
  - `front`
  - `back`
- **Iterators:**
  - `begin`
  - `end`
  ```
  #include <iostream>
  #include <deque>

  int main() {
      std::deque<int> myDeque;

      // Modifiers
      myDeque.push_back(1);
      myDeque.push_front(2);
      myDeque.pop_back();
      myDeque.pop_front();
      myDeque.emplace_back(3);
      myDeque.emplace_front(4);
      myDeque.insert(myDeque.begin() + 1, 5);
      myDeque.erase(myDeque.begin());
      myDeque.clear();

      // Capacity
      bool isEmpty = myDeque.empty();
      int size = myDeque.size();

      // Element Access
      int frontElement = myDeque.front();
      int backElement = myDeque.back();
      int elementAtIndex = myDeque[0];
      int elementAt = myDeque.at(1);

      // Iterators
      auto it = myDeque.begin();
      auto endIt = myDeque.end();

      return 0;
  }

  ```

### priority_queue in C++ STL:

- **Modifiers:**
  - `push`
  - `pop`
- **Capacity:**
  - `empty`
  - `size`
- **Element Access:**
  - `top`

  ```
  #include <iostream>
  #include <queue>

  int main() {
      std::priority_queue<int> myPriorityQueue;

      // Modifiers
      myPriorityQueue.push(3);
      myPriorityQueue.push(1);
      myPriorityQueue.push(5);
      myPriorityQueue.push(2);
      myPriorityQueue.pop(); // Removes the top element (5)

      // Capacity
      bool isEmpty = myPriorityQueue.empty();
      int size = myPriorityQueue.size();

      // Element Access
      int topElement = myPriorityQueue.top(); // Returns the top element (3)

      return 0;
  }

  ```

### multimap in C++ STL:

(Functions are similar to map)

### list in C++ STL:

- **Modifiers:**
  - `push_back`
  - `push_front`
  - `pop_back`
  - `pop_front`
  - `emplace_back`
  - `emplace_front`
  - `insert`
  - `erase`
  - `clear`
- **Capacity:**
  - `empty`
  - `size`
- **Iterators:**
  - `begin`
  - `end`
- **Operations:**
  - `sort`
  - `reverse`
  - `splice`
  - `merge`
  - `remove`
  - `remove_if`
  - `unique`
  ```
  #include <iostream>
  #include <list>

  int main() {
      std::list<int> myList;

      // Modifiers
      myList.push_back(1);
      myList.push_front(2);
      myList.pop_back();
      myList.pop_front();
      myList.emplace_back(3);
      myList.emplace_front(4);
      myList.insert(myList.begin() + 1, 5);
      myList.erase(myList.begin());
      myList.clear();

      // Capacity
      bool isEmpty = myList.empty();
      int size = myList.size();

      // Iterators
      auto it = myList.begin();
      auto endIt = myList.end();

      // Operations
      myList.sort();
      myList.reverse();
      // Other operations like splice, merge, remove, remove_if, unique can also be performed

      return 0;
  }

  ```

### next_permutation in STL:

- **Algorithm:**
  - `next_permutation`

### __builtin_popcount() in STL:

- **Bit Manipulation:**
  - `__builtin_popcount`

### sort() in C++ STL:

- **Algorithm:**
  - `sort`

### min_element() in C++ STL:

- **Algorithm:**
  - `min_element`

### max_element() in C++ STL:

- **Algorithm:**
  - `max_element`
