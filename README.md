# rotate-image-
 void rotate(vector<vector<int>>& arr) {
        int n = arr.size();
        for(int i =0;i<n;i++){
            for(int j= i+1;j<n;j++){
                swap(arr[i][j], arr[j][i]);
            }
        }
        
        for(int i =0;i<n;i++){
            for(int j = 0;j<n/2;j++){
                swap(arr[i][j] , arr[i][(n-1)-j]);
            }
        }
    }
};
