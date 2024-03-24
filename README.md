# Find-even-sum
You're given two set of cards, first set contains N even numbered cards and the other set contains M odd cards. Find the number of ways to choose two cards out of total N + M cards, such that their sum is even.  Input The first and the only line of the input contains 2 space separated integers, N and M  Constraints: 1) 0 ≤ N, M ≤ 100 2) 2 ≤ N + M

def even_sum_ways(N, M):
    case1 = N * (N - 1) // 2   
    case2 = M * (M - 1) // 2
    return case1 + case2

N, M = map(int, input().split())

print(even_sum_ways(N, M))
