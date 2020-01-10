# problem-solving
Compare the triplets function solution in C
int* compareTriplets(int a_count, int* a, int b_count, int* b, int* result_count) 
{
    * result_count = 2;
    static int arr[2];

    int i,x=0,y=0;
    for(i=0 ; i<3 ; i++)
    {
        if(a[i] > b[i])
        {
            x++;
        }
        else if(a[i] < b[i])
        {
            y++;
        }
        else if(a[i] == b[i])
        {
            continue;
        }
    }

arr[0] = x;
arr[1]=y;



return arr;
}
