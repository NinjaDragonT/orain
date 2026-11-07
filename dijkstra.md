<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# Thuật toán Dijkstra

**Độ phức tạp:** $O(V + E \log V)$ nếu dùng Hàng đợi ưu tiên (Priority Queue).

## Ý tưởng cơ bản
Thuật toán dùng để tìm đường đi ngắn nhất từ 1 đỉnh nguồn đến các đỉnh còn lại trên đồ thị có trọng số không âm.

## Cài đặt bằng C++

```cpp
#include <bits/stdc++.h>
using namespace std;

const int INF = 1e9;
vector<pair<int, int>> adj[1000];
int d[1000];

void dijkstra(int start) {
    // Code của bạn ở đây...
}
