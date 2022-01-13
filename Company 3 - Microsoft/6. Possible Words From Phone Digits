class Solution
{
    public:
    vector<string> ch = {"", "", "abc", "def", "ghi", "jkl", "mno", "pqrs", "tuv", "wxyz"};
    vector<string> ans;
    string s;
    
    void solve(int a[], int n, string &s, int index = 0)
    {
        if(index >= n){
            ans.push_back(s);
            return;
        }
        
        string curr = ch[a[index]];
        for(int i=0; i<curr.length(); i++)
        {
            s.push_back(curr[i]);
            solve(a, n, s, index+1);
            // ans.push_back(s);
            s.pop_back();
        }
    }
    
    vector<string> possibleWords(int a[], int n)
    {
        //Your code here
        solve(a, n, s);
        return ans;
    }
};
