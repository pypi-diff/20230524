# Comparing `tmp/packagetenssor-0.5.tar.gz` & `tmp/packagetenssor-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packagetenssor-0.5.tar", last modified: Mon May 22 05:55:57 2023, max compression
+gzip compressed data, was "packagetenssor-0.6.tar", last modified: Wed May 24 04:32:29 2023, max compression
```

## Comparing `packagetenssor-0.5.tar` & `packagetenssor-0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        0 2023-05-22 05:55:57.188758 packagetenssor-0.5/
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      215 2023-05-22 05:55:57.188400 packagetenssor-0.5/PKG-INFO
-drwxr-xr-x   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        0 2023-05-22 05:55:57.186501 packagetenssor-0.5/packagetenssor.egg-info/
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      215 2023-05-22 05:55:57.000000 packagetenssor-0.5/packagetenssor.egg-info/PKG-INFO
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      180 2023-05-22 05:55:57.000000 packagetenssor-0.5/packagetenssor.egg-info/SOURCES.txt
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        1 2023-05-22 05:55:57.000000 packagetenssor-0.5/packagetenssor.egg-info/dependency_links.txt
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        8 2023-05-22 05:55:57.000000 packagetenssor-0.5/packagetenssor.egg-info/top_level.txt
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)       38 2023-05-22 05:55:57.188820 packagetenssor-0.5/setup.cfg
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      258 2023-05-22 05:55:46.000000 packagetenssor-0.5/setup.py
-drwxr-xr-x   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        0 2023-05-22 05:55:57.187457 packagetenssor-0.5/tenssor/
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)    31114 2023-05-22 05:54:15.000000 packagetenssor-0.5/tenssor/__init__.py
+drwxr-xr-x   0 ankit.sharma10 (101996570) 1493847943        0 2023-05-24 04:32:29.888619 packagetenssor-0.6/
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      215 2023-05-24 04:32:29.887427 packagetenssor-0.6/PKG-INFO
+drwxr-xr-x   0 ankit.sharma10 (101996570) 1493847943        0 2023-05-24 04:32:29.875800 packagetenssor-0.6/packagetenssor.egg-info/
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      215 2023-05-24 04:32:29.000000 packagetenssor-0.6/packagetenssor.egg-info/PKG-INFO
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      180 2023-05-24 04:32:29.000000 packagetenssor-0.6/packagetenssor.egg-info/SOURCES.txt
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943        1 2023-05-24 04:32:29.000000 packagetenssor-0.6/packagetenssor.egg-info/dependency_links.txt
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943        8 2023-05-24 04:32:29.000000 packagetenssor-0.6/packagetenssor.egg-info/top_level.txt
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943       38 2023-05-24 04:32:29.888827 packagetenssor-0.6/setup.cfg
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943      258 2023-05-24 04:32:17.000000 packagetenssor-0.6/setup.py
+drwxr-xr-x   0 ankit.sharma10 (101996570) 1493847943        0 2023-05-24 04:32:29.886046 packagetenssor-0.6/tenssor/
+-rw-r--r--   0 ankit.sharma10 (101996570) 1493847943    34142 2023-05-24 04:29:50.000000 packagetenssor-0.6/tenssor/__init__.py
```

### Comparing `packagetenssor-0.5/tenssor/__init__.py` & `packagetenssor-0.6/tenssor/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -555,452 +555,566 @@
 """
 
 print('RMSE in terms of % of the orignal value is', round((rmse/real_stock_price_test.mean()*100), 2) , '%')   
 # we take the avg because it would be a true representative of the real stock values
 '''
 
 s5 = '''
-#include<bits/stdc++.h>
-#include<omp.h>
-#include<chrono>
+#include <bits/stdc++.h>
+
 using namespace std;
-using namespace std::chrono;
 
-int N = 10, M = 10;
-vector<int> graph [10];
-void bfs_p(int start) {
-	vector<bool> vis(N);
-	queue<int> q;
-	q.push(start);
-
-	while(!q.empty()) {
-		int cur = q.front();
-		q.pop();
-		if(!vis[cur]) {
-			vis[cur] = 1; cout << cur <<" ";
-			
-			#pragma omp parallel for
-			for (int next: graph[cur]) {
-				if(!vis[next]) q.push(next);			
-			}		
-		}	
-	}
-}
-
-void bfs(int start) {
-	vector<bool> vis(N);
-	queue<int> q;
-	q.push(start);
-
-	while(!q.empty()) {
-		int cur = q.front();
-		q.pop();
-		if(!vis[cur]) {
-			vis[cur] = 1; cout << cur <<" ";
-			
-			for (int next: graph[cur]) {
-				if(!vis[next]) q.push(next);			
-			}		
-		}	
-	}
-}
-
-void dfs_p(int start) {
-	vector<bool> vis(N);
-	stack<int> q;
-	q.push(start);
-
-	while(!q.empty()) {
-		int cur = q.top();
-		q.pop();
-		if(!vis[cur]) {
-			vis[cur] = 1; cout << cur <<" ";
-			
-			#pragma omp parallel for
-			for (int next: graph[cur]) {
-				if(!vis[next]) q.push(next);			
-			}		
-		}	
-	}
-}
-void dfs(int start) {
-	vector<bool> vis(N);
-	stack<int> q;
-	q.push(start);
-
-	while(!q.empty()) {
-		int cur = q.top();
-		q.pop();
-		if(!vis[cur]) {
-			vis[cur] = 1; cout << cur <<" ";
-			
-			for (int next: graph[cur]) {
-				if(!vis[next]) q.push(next);			
-			}		
-		}	
-	}
+// Function to perform Parallel BFS
+void parallelBFS(vector<vector<int>>& adj_list, int source, vector<bool>& visited, vector<int>& bfs_order) {
+    queue<int> q;
+    q.push(source);
+
+    // Parallel loop over the queue
+    #pragma omp parallel
+    {
+        while (!q.empty()) {
+            // Get the next vertex from the queue
+            #pragma omp for
+            for (int i = 0; i < q.size(); i++) {
+                int curr = q.front();
+                q.pop();
+
+                // If the current vertex has not been visited, mark it as visited
+                // and explore all its neighbors
+                if (!visited[curr]) {
+                    #pragma omp critical
+                    {
+                        visited[curr] = true;
+                        bfs_order.push_back(curr); // add the visited node to the bfs_order vector
+                    }
+                    for (int j = 0; j < adj_list[curr].size(); j++) {
+                        int neighbor = adj_list[curr][j];
+
+                        // Add the neighbor to the queue if it has not been visited
+                        if (!visited[neighbor]) {
+                            q.push(neighbor);
+                        }
+                    }
+                }
+            }
+        }
+    }
+}
+
+// Function to perform Parallel DFS
+void parallelDFS(vector<vector<int>>& adj_list, int source, vector<bool>& visited, vector<int>& dfs_order) {
+    stack<int> s;
+    s.push(source);
+
+    // Parallel loop over the stack
+    #pragma omp parallel
+    {
+        while (!s.empty()) {
+            // Get the next vertex from the stack
+            #pragma omp for
+            for (int i = 0; i < s.size(); i++) {
+                int curr = s.top();
+                s.pop();
+
+                // If the current vertex has not been visited, mark it as visited
+                // and explore all its neighbors
+                if (!visited[curr]) {
+                    #pragma omp critical
+                    {
+                        visited[curr] = true;
+                        dfs_order.push_back(curr); // add the visited node to the dfs_order vector
+                    }
+                    for (int j = 0; j < adj_list[curr].size(); j++) {
+                        int neighbor = adj_list[curr][j];
+
+                        // Add the neighbor to the stack if it has not been visited
+                        if (!visited[neighbor]) {
+                            s.push(neighbor);
+                        }
+                    }
+                }
+            }
+        }
+    }
 }
 
 int main() {
-	cout << "Enter 4 edges :" << endl;
-	for(int i = 0; i < 4; i++) {
-		int x, y; cin >> x >> y;
-		graph[x].push_back(y);
-		graph[y].push_back(x);	
-	}
-//~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-	cout << "Paralel BFS traversal : ";
-
-	auto start = high_resolution_clock::now();
-	bfs_p(0);
-	cout << endl;
-	auto end = high_resolution_clock::now();
-	auto dur = duration_cast<microseconds>(end - start);
-	cout << "Time taken : " <<dur.count() << " ms" <<endl; 
-
-//~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-	cout << "Normal BFS traversal : ";
-
-	start = high_resolution_clock::now();
-	bfs(0);
-	cout << endl;
-	end = high_resolution_clock::now();
-	dur = duration_cast<microseconds>(end - start);
-	cout << "Time taken : " <<dur.count() << " ms" <<endl; 
-
-//~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~	
-	cout << "Paralel DFS traversal : ";
-	start = high_resolution_clock::now();
-	dfs_p(0);
-	cout << endl;
-	end = high_resolution_clock::now();
-	dur = duration_cast<microseconds>(end - start);
-	cout << "Time taken : " <<dur.count() << " ms" <<endl; 
-//~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~	
-	cout << "Common DFS traversal : ";
-	start = high_resolution_clock::now();
-	dfs(0);
-	cout << endl;
-	end = high_resolution_clock::now();
-	dur = duration_cast<microseconds>(end - start);
-	cout << "Time taken : " <<dur.count() << " ms" <<endl; 
-	
+    // Construct the adjacency list
+    vector<vector<int>> adj_list = {
+        {1, 2},
+        {0, 3, 4},
+        {0, 5, 6},
+        {1},
+        {1},
+        {2},
+        {2}
+    };
+
+    // Perform Parallel BFS from node 0
+    int source = 0;
+    int n = adj_list.size();
+    vector<bool> visited(n, false);
+    vector<int> bfs_order;
+    parallelBFS(adj_list, source, visited, bfs_order);
+
+    // Print the visited nodes and the BFS order
+    cout << "BFS order: ";
+    for (int i = 0; i < bfs_order.size(); i++) {
+        cout << bfs_order[i] << " ";
+    }
+    cout << endl;
+
+    for (int i = 0; i < n; i++) {
+        if (visited[i]) {
+            cout << "Node " << i << " has been visited" << endl;
+        }
+    }
+
+    // Perform Parallel DFS from
+// reset the visited vector
+fill(visited.begin(), visited.end(), false);
+vector<int> dfs_order;
+parallelDFS(adj_list, source, visited, dfs_order);
+
+// Print the visited nodes and the DFS order
+cout << "DFS order: ";
+for (int i = 0; i < dfs_order.size(); i++) {
+    cout << dfs_order[i] << " ";
+}
+cout << endl;
+
+for (int i = 0; i < n; i++) {
+    if (visited[i]) {
+        cout << "Node " << i << " has been visited" << endl;
+    }
+}
+
+return 0;
 }
 '''
 
 s6 = '''
-#include <bits/stdc++.h>
+#include <iostream>
+#include <cstdlib>
+#include <ctime>
+#include <iomanip>
 #include <omp.h>
-#include<chrono>
+
 using namespace std;
-using namespace std::chrono;
+void parallel_bubble_sort_odd_even(int arr[], int n) {
+    int phase, i, temp;
+    for (phase = 0; phase < n; phase++) {
+        if (phase % 2 == 0) {  // Even phase
+            #pragma omp parallel for private(i, temp)
+            for (i = 2; i < n; i += 2) {
+                if (arr[i - 1] > arr[i]) {
+                    temp = arr[i - 1];
+                    arr[i - 1] = arr[i];
+                    arr[i] = temp;
+                }
+            }
+        } else {  // Odd phase
+            #pragma omp parallel for private(i, temp)
+            for (i = 1; i < n; i += 2) {
+                if (arr[i - 1] > arr[i]) {
+                    temp = arr[i - 1];
+                    arr[i - 1] = arr[i];
+                    arr[i] = temp;
+                }
+            }
+        }
+    }
+}
 
-int N = 6;
 
-void bubble_sort_p(int a[], int n) {
-	#pragma omp parallel shared (a, n)
-	{
-		int i,j;
-		#pragma omp for
-		for(int i = 0; i < n-1; i++) {
-			for(j = 0; j < n-i-1; j++) {
-				if(a[j] > a[j+1]) swap(a[j], a[j+1]);			
-			} 		
-		}
-	}
-}
-
-
-void bubble_sort(int a[], int n) {
-
-	{
-		int i,j;
-
-		for(int i = 0; i < n-1; i++) {
-			for(j = 0; j < n-i-1; j++) {
-				if(a[j] > a[j+1]) swap(a[j], a[j+1]);			
-			} 		
-		}
-	}
-}
-void merge(int a[], int l, int md, int r) {
-	vector<int> temp(r - l + 1);
-	int i = l, j = md + 1, k = 0;
-	
-	while(i <= md && j <= r) {
-		if(a[i] <= a[j]) temp[k++] = a[i++];
-		else temp[k++] = a[j++];
-	} 
-
-	while(i <= md) temp[k++] = a[i++];
-	while(j <= r) temp[k++] = a[j++];
-	
-	for(int i = 0; i < k; i++) a[l+i] = temp[i];
-
-}
-
-void merge_sort_p(int a[], int l, int r) {
-	if( l < r){
-		int md = (l + r) / 2;
-		#pragma omp parallel sections 
-		{
-			#pragma omp section
-				merge_sort_p(a, l, md);
-			#pragma omp section
-				merge_sort_p(a, md + 1, r);
- 			
-			merge(a, l, md, r);		
-		}
-	}
-}
-
-void merge_sort(int a[], int l, int r) {
-	if( l < r){
-		int md = (l + r) / 2;
-
-		{
-
-				merge_sort(a, l, md);
-
-				merge_sort(a, md + 1, r);
- 			
-			merge(a, l, md, r);		
-		}
-	}
+void bubble_sort(int arr[], int n) {
+    int i, j;
+    for (i = 0; i < n - 1; i++) {
+        for (j = 0; j < n - i - 1; j++) {
+            if (arr[j] > arr[j + 1]) {
+                swap(arr[j], arr[j + 1]);
+            }
+        }
+    }
+}
+
+void merge(int arr[], int l, int m, int r) {
+    int n1 = m - l + 1;
+    int n2 = r - m;
+
+    int L[n1], R[n2];
+    int i, j, k;
+
+    for (i = 0; i < n1; i++)
+        L[i] = arr[l + i];
+    for (j = 0; j < n2; j++)
+        R[j] = arr[m + 1 + j];
+
+    i = 0;
+    j = 0;
+    k = l;
+    while (i < n1 && j < n2) {
+        if (L[i] <= R[j]) {
+            arr[k] = L[i];
+            i++;
+        }
+        else {
+            arr[k] = R[j];
+            j++;
+        }
+        k++;
+    }
+
+    while (i < n1) {
+        arr[k] = L[i];
+        i++;
+        k++;
+    }
+
+    while (j < n2) {
+        arr[k] = R[j];
+        j++;
+        k++;
+    }
+}
+
+void merge_sort(int arr[], int l, int r) {
+    if (l < r) {
+        int m = l + (r - l) / 2;
+
+        #pragma omp parallel sections
+        {
+            #pragma omp section
+            {
+                merge_sort(arr, l, m);
+            }
+
+            #pragma omp section
+            {
+                merge_sort(arr, m + 1, r);
+            }
+        }
+
+        merge(arr, l, m, r);
+    }
+}
+
+void print_array(int arr[], int n) {
+    for (int i = 0; i < n; i++) {
+        cout << arr[i] << " ";
+    }
+    cout << endl;
 }
 
 int main() {
-	cout << "Enter " << N << " elements: ";
-	int a[N], a1[N], a2[N], a3[N];	
-	for(int i = 0; i < N; i++) {cin >> a[i]; a1[i] = a[i]; a2[i] = a[i]; a3[i] = a[i];  }
-//~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-	cout << "Array after normal Bubble sort: ";
-	auto start = high_resolution_clock::now();
-	bubble_sort(a, N);
-	auto end = high_resolution_clock::now();
-	auto dur = duration_cast<microseconds>(end - start);
-	for(int i = 0; i < N; i++) {cout << a[i] <<" ";} cout << endl;
-
-	cout << "Time taken : " <<dur.count() << " ms" <<endl; 	
-
-//~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-	cout << "Array after parallel Bubble sort: ";
-	start = high_resolution_clock::now();
-	bubble_sort_p(a1, N);
-	end = high_resolution_clock::now();
-	dur = duration_cast<microseconds>(end - start);
-	for(int i = 0; i < N; i++) {cout << a1[i] <<" ";} cout << endl;
-
-	cout << "Time taken : " <<dur.count() << " ms" <<endl; 	
-
-
-//~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-	cout << "Array after normal Merge sort: ";
-	start = high_resolution_clock::now();
-	merge_sort(a2, 0, N-1);
-	end = high_resolution_clock::now();
-	dur = duration_cast<microseconds>(end - start);
-	for(int i = 0; i < N; i++) {cout << a2[i] << " ";} cout << endl;
-	cout << "Time taken : " <<dur.count() << " ms" <<endl; 	
-//~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~	
-	cout << "Array after parallel Merge sort: ";
-	start = high_resolution_clock::now();
-	merge_sort_p(a3, 0, N-1);
-	end = high_resolution_clock::now();
-	dur = duration_cast<microseconds>(end - start);
-	for(int i = 0; i < N; i++) {cout << a3[i] << " ";} cout << endl;
-	cout << "Time taken : " <<dur.count() << " ms" <<endl; 	
-//~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~	
-  
+    srand(time(NULL));
+
+    int n = 10000;
+    int arr[n];
+
+    for (int i = 0; i < n; i++) {
+        arr[i] = rand() % 10000;
+    }
+
+    double start_time, end_time;
+
+    cout << "Sequential Bubble Sort" << endl;
+    start_time = omp_get_wtime();
+    bubble_sort(arr, n);
+    end_time = omp_get_wtime();
+    cout << "Time taken: " << end_time - start_time << " seconds" << endl;
+
+    for (int i = 0; i < n; i++) {
+        arr[i] = rand() % 10000;
+    }
+
+    cout << "Parallel Bubble Sort" << endl;
+    start_time = omp_get_wtime();
+    #pragma omp parallel
+    {
+        parallel_bubble_sort_odd_even(arr, n);
+    }
+    end_time = omp_get_wtime();
+    cout << "Time taken: " << end_time - start_time << " seconds" << endl;
+
+    for (int i = 0; i < n; i++) {
+       arr[i] = rand() % 10000;
+}
+
+cout << "Sequential Merge Sort" << endl;
+start_time = omp_get_wtime();
+merge_sort(arr, 0, n - 1);
+end_time = omp_get_wtime();
+cout << "Time taken: " << end_time - start_time << " seconds" << endl;
+
+for (int i = 0; i < n; i++) {
+    arr[i] = rand() % 10000;
+}
+
+cout << "Parallel Merge Sort" << endl;
+start_time = omp_get_wtime();
+#pragma omp parallel
+{
+    #pragma omp single nowait
+    {
+        merge_sort(arr, 0, n - 1);
+    }
+}
+end_time = omp_get_wtime();
+cout << "Time taken: " << end_time - start_time<<setprecision(20) <<" seconds" << endl;
+
+return 0;
 }
 '''
 
 s7 = '''
 #include <bits/stdc++.h>
+#include <ctime>
 #include <omp.h>
 
 using namespace std;
 
-int N = 6, a[100];
-
-void max_red(int a[], int n) {
-	int mx = INT_MIN;
-	
-	#pragma omp parallel for reduction(max: mx)
-	for(int i = 0; i < n; i++) if(a[i] > mx) mx = a[i];
-	
-	cout << "Maximum value: " << mx << endl; 
-}
-void min_red(int a[], int n) {
-	int mn = INT_MAX;
-	
-	#pragma omp parallel for reduction(min: mn)
-	for(int i = 0; i < n; i++) if(a[i] < mn) mn = a[i];
-	
-	cout << "Minimum value: " << mn << endl; 
+// Parallel reduction to find min value
+template<typename T> T parallel_min(const vector<T>& data)
+{
+    T min_value = data[0];
+    #pragma omp parallel for reduction(min:min_value)
+    for (int i = 1; i < data.size(); ++i)
+        if (data[i] < min_value)
+            min_value = data[i];
+
+    return min_value;
+}
+
+// Parallel reduction to find max value
+template<typename T> T parallel_max(const vector<T>& data)
+{
+    T max_value = data[0];
+    #pragma omp parallel for reduction(max:max_value)
+    for (int i = 1; i < data.size(); ++i)
+        if (data[i] > max_value)
+            max_value = data[i];
+    return max_value;
+}
+
+// Parallel reduction to find sum
+template<typename T> T parallel_sum(const vector<T>& data)
+{
+    T sum = 0;
+    #pragma omp parallel for reduction(+:sum)
+    for (int i = 0; i < data.size(); ++i)
+        sum += data[i];
+
+    return sum;
+}
+
+// Parallel reduction to find average
+template<typename T> double parallel_average(const vector<T>& data)
+{
+    T sum = parallel_sum(data);
+    double average = static_cast<double>(sum) / data.size();
+    return average;
 }
 
+int main() {
+    // Ask user for the size of the vector
+    int size;
+    cout << "Enter the size of the vector: ";
+    cin >> size;
+
+    // Ask user for the values of the vector
+    vector<int> data(size);
+    cout << "Enter the values of the vector:" << endl;
+    for (int i = 0; i < size; ++i) {
+        cin >> data[i];
+    }
 
-void sum_red(int a[], int n) {
-	int sum = 0;
-	
-	#pragma omp parallel for reduction(+: sum)
-	for(int i = 0; i < n; i++) sum += a[i];
-	
-	cout << "Sum: " << sum << endl; 
-}
+    // Find min, max, sum and average using parallel reduction
+    auto start_time = chrono::steady_clock::now();
 
+    int min_value = parallel_min(data);
+    int max_value = parallel_max(data);
+    int sum = parallel_sum(data);
+    double average = parallel_average(data);
+
+    auto end_time = chrono::steady_clock::now();
+
+    // Print results and timing information
+    cout << "Min value: " << min_value << endl;
+    cout << "Max value: " << max_value << endl;
+    cout << "Sum: " << sum << endl;
+    cout << "Average: " << average << endl;
+    auto duration_ms = chrono::duration_cast<chrono::milliseconds>(end_time - start_time);
+    cout << "Time taken: " << duration_ms.count() << "ms" << endl;
 
-void avg_red(int a[], int n) {
-	double sum = 0, cnt = n;
-	
-	#pragma omp parallel for reduction(+: sum)
-	for(int i = 0; i < n; i++) sum += a[i];
-	double avg = sum / cnt;
-	cout << "Average: " << avg << endl; 
+    return 0;
 }
-
-int main() {
-	cout << "Enter " << N << " elements: ";
-	int a[N] ;	
-	for(int i = 0; i < N; i++) cin >> a[i];
-	
-	max_red(a, N);
-	min_red(a, N);
-	sum_red(a, N);
-	avg_red(a, N);
-	max_red(a, N);
-}
-
-/* 
-Sample Input :
-3 1 8 0 5
-
-*/
 '''
 
 s8 = '''
 #include <iostream>
-#include <vector>
+#include <cstdlib>
+#include <cstdio>
+#include <ctime>
 
-// CUDA kernel function for vector addition
-__global__ void vectorAddition(const float* a, const float* b, float* result, int size) {
-    int index = blockIdx.x * blockDim.x + threadIdx.x;
+#define TILE_WIDTH 32
 
-    if (index < size) {
-        result[index] = a[index] + b[index];
+__global__ void matrixMult(int *a, int *b, int *c, int n)
+{
+    int row = blockIdx.y * blockDim.y + threadIdx.y;
+    int col = blockIdx.x * blockDim.x + threadIdx.x;
+
+    if (row < n && col < n) {
+        int sum = 0;
+        for (int i = 0; i < n; ++i) {
+            sum += a[row * n + i] * b[i * n + col];
+        }
+        c[row * n + col] = sum;
     }
 }
 
-int main() {
-    int size = 1000000;  // Size of the vectors
-    std::vector<float> a(size, 1.0f);  // Vector a initialized with 1.0
-    std::vector<float> b(size, 2.0f);  // Vector b initialized with 2.0
-    std::vector<float> result(size);   // Result vector
-
-    // Declare device pointers
-    float* d_a;
-    float* d_b;
-    float* d_result;
-
-    // Allocate memory on the device
-    cudaMalloc(&d_a, size * sizeof(float));
-    cudaMalloc(&d_b, size * sizeof(float));
-    cudaMalloc(&d_result, size * sizeof(float));
-
-    // Copy input vectors from host to device
-    cudaMemcpy(d_a, a.data(), size * sizeof(float), cudaMemcpyHostToDevice);
-    cudaMemcpy(d_b, b.data(), size * sizeof(float), cudaMemcpyHostToDevice);
-
-    // Define the grid and block sizes
-    int blockSize = 256;
-    int gridSize = (size + blockSize - 1) / blockSize;
-
-    // Launch the kernel on the GPU
-    vectorAddition<<<gridSize, blockSize>>>(d_a, d_b, d_result, size);
-
-    // Copy the result vector from device to host
-    cudaMemcpy(result.data(), d_result, size * sizeof(float), cudaMemcpyDeviceToHost);
+int main()
+{
+    int n;
+    n=4;
+
+    // allocate memory for matrices on host
+    int *a = new int[n * n];
+    int *b = new int[n * n];
+    int *c = new int[n * n];
+
+    // initialize matrices with random values
+    std::srand(std::time(0));
+    for (int i = 0; i < n * n; ++i) {
+        a[i] = std::rand() % 10;
+        b[i] = std::rand() % 10;
+    }
 
-    // Print the result
-    for (int i = 0; i < size; ++i) {
-        std::cout << result[i] << " ";
+    // allocate memory for matrices on device
+    int *dev_a, *dev_b, *dev_c;
+    cudaMalloc(&dev_a, n * n * sizeof(int));
+    cudaMalloc(&dev_b, n * n * sizeof(int));
+    cudaMalloc(&dev_c, n * n * sizeof(int));
+
+    // copy matrices from host to device
+    cudaMemcpy(dev_a, a, n * n * sizeof(int), cudaMemcpyHostToDevice);
+    cudaMemcpy(dev_b, b, n * n * sizeof(int), cudaMemcpyHostToDevice);
+
+    // launch kernel
+    dim3 dimGrid((n - 1) / TILE_WIDTH + 1, (n - 1) / TILE_WIDTH + 1, 1);
+    dim3 dimBlock(TILE_WIDTH, TILE_WIDTH, 1);
+    matrixMult<<<dimGrid, dimBlock>>>(dev_a, dev_b, dev_c, n);
+
+    // copy result matrix from device to host
+    cudaMemcpy(c, dev_c, n * n * sizeof(int), cudaMemcpyDeviceToHost);
+
+    // print result matrix
+ std::cout << "Result matrix:\n";
+    for (int i = 0; i < n; ++i) {
+        for (int j = 0; j < n; ++j) {
+            std::cout << a[i * n + j] << " ";
+        }
+        std::cout << "\n";
+    }
+ std::cout << "Result matrix:\n";
+    for (int i = 0; i < n; ++i) {
+        for (int j = 0; j < n; ++j) {
+            std::cout << b[i * n + j] << " ";
+        }
+        std::cout << "\n";
+    }
+    std::cout << "Result matrix:\n";
+    for (int i = 0; i < n; ++i) {
+        for (int j = 0; j < n; ++j) {
+            std::cout << c[i * n + j] << " ";
+        }
+        std::cout << "\n";
     }
-    std::cout << std::endl;
 
-    // Free device memory
-    cudaFree(d_a);
-    cudaFree(d_b);
-    cudaFree(d_result);
+    // free memory on device
+    cudaFree(dev_a);
+    cudaFree(dev_b);
+    cudaFree(dev_c);
+
+    // free memory on host
+    delete[] a;
+    delete[] b;
+    delete[] c;
 
     return 0;
 }
 '''
 
 s9 = '''
-
 #include <iostream>
 #include <vector>
+#include <cstdlib>
+#include <ctime>
 
-// CUDA kernel function for matrix multiplication
-__global__ void matrixMultiplication(const float* a, const float* b, float* result, int size) {
-    int row = blockIdx.y * blockDim.y + threadIdx.y;
-    int col = blockIdx.x * blockDim.x + threadIdx.x;
+using namespace std;
 
-    if (row < size && col < size) {
-        float sum = 0.0f;
-        for (int k = 0; k < size; ++k) {
-            sum += a[row * size + k] * b[k * size + col];
-        }
-        result[row * size + col] = sum;
+__global__ void vector_add(int *a, int *b, int *c, int n) {
+    int i = threadIdx.x + blockIdx.x * blockDim.x;
+    if (i < n) {
+        c[i] = a[i] + b[i];
     }
 }
 
 int main() {
-    int size = 1000;  // Size of the matrices
-    std::vector<float> a(size * size, 1.0f);  // Matrix a initialized with 1.0
-    std::vector<float> b(size * size, 2.0f);  // Matrix b initialized with 2.0
-    std::vector<float> result(size * size);   // Result matrix
-
-    // Declare device pointers
-    float* d_a;
-    float* d_b;
-    float* d_result;
-
-    // Allocate memory on the device
-    cudaMalloc(&d_a, size * size * sizeof(float));
-    cudaMalloc(&d_b, size * size * sizeof(float));
-    cudaMalloc(&d_result, size * size * sizeof(float));
-
-    // Copy input matrices from host to device
-    cudaMemcpy(d_a, a.data(), size * size * sizeof(float), cudaMemcpyHostToDevice);
-    cudaMemcpy(d_b, b.data(), size * size * sizeof(float), cudaMemcpyHostToDevice);
-
-    // Define the block and grid sizes
-    dim3 blockSize(16, 16);
-    dim3 gridSize((size + blockSize.x - 1) / blockSize.x, (size + blockSize.y - 1) / blockSize.y);
-
-    // Launch the kernel on the GPU
-    matrixMultiplication<<<gridSize, blockSize>>>(d_a, d_b, d_result, size);
-
-    // Copy the result matrix from device to host
-    cudaMemcpy(result.data(), d_result, size * size * sizeof(float), cudaMemcpyDeviceToHost);
-
-    // Print the result (Optional)
-    // for (int i = 0; i < size; ++i) {
-    //     for (int j = 0; j < size; ++j) {
-    //         std::cout << result[i * size + j] << " ";
-    //     }
-    //     std::cout << std::endl;
-    // }
+    const int n = 100;  // Length of vectors
+    std::vector<int> a(n), b(n), c(n);
 
-    // Free device memory
+    // Initialize vectors with random values
+    std::srand(std::time(nullptr));
+    for (int i = 0; i < n; ++i) {
+        a[i] = std::rand() % 100;
+        b[i] = std::rand() % 100;
+    }
+
+    // Allocate memory on device
+    int *d_a, *d_b, *d_c;
+    cudaMalloc(&d_a, n * sizeof(int));
+    cudaMalloc(&d_b, n * sizeof(int));
+    cudaMalloc(&d_c, n * sizeof(int));
+
+    // Copy input data from host to device
+    cudaMemcpy(d_a, a.data(), n * sizeof(int), cudaMemcpyHostToDevice);
+    cudaMemcpy(d_b, b.data(), n * sizeof(int), cudaMemcpyHostToDevice);
+
+    // Launch kernel
+    const int block_size = 256;
+    const int num_blocks = (n + block_size - 1) / block_size;
+    vector_add<<<num_blocks, block_size>>>(d_a, d_b, d_c, n);
+
+    // Copy output data from device to host
+    cudaMemcpy(c.data(), d_c, n * sizeof(int), cudaMemcpyDeviceToHost);
+
+    // Free memory on device
     cudaFree(d_a);
     cudaFree(d_b);
-    cudaFree(d_result);
+    cudaFree(d_c);
+
+    // Print results
+    std::cout << "Vector a: ";
+    for (int i = 0; i < n; ++i) {
+        std::cout << a[i] << " ";
+    }
+    std::cout << std::endl;
+
+    std::cout << "Vector b: ";
+    for (int i = 0; i < n; ++i) {
+        std::cout << b[i] << " ";
+    }
+    std::cout << std::endl;
+
+    std::cout << "Vector c: ";
+    for (int i = 0; i < n; ++i) {
+        std::cout << c[i] << " ";
+    }
+    std::cout << std::endl;
 
     return 0;
 }
 '''
 
 s10 = '''
 #include<bits/stdc++.h>
```

