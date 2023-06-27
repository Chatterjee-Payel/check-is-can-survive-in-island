# check-is-can-survive-in-island

class Solution{
public:
    int minimumDays(int S, int N, int M){
        // code here
        int sunday=S/7;
        int buy_days=S-sunday;
        int tot_food=S*M;
        int ans=0;
        if(tot_food%N==0)
        {
            ans=tot_food/N;
            
        }
        else{
            ans=tot_food/N+1;
            
        }
        if(ans<=buy_days)
        {
            return ans;
        }
        else{
            return -1;
        }
    }
};
