### 刷题链接：
leetcode中文网：https://leetcode-cn.com/  
leetcode英文网：https://leetcode.com/   
Top100常见题：https://leetcode.com/problemset/top-100-liked-questions/    

### 刷题记录：
|题目|难度|时间复杂度|类型|完成度|方法|
|--|--|--|--|--|--|--|
|1.两数之和|Easy|$O(n)$|数组、哈希表|Done|保存字典，判断差是否在字典中出现过，注意索引|
|2.两数相加|Medium|$O(m+n)$|链表|No|模拟加法的实现，注意进位|
|3.无重复字符的最长子串|Medium|$O(n)$|字符串|No|字典保存字符位置，判断是否在字典中出现过|
|4.两个有序数组的中位数|Medium|$O(log(m+n))$|数学|No|二分法，依次删除不满足条件的k/2个值|
|5.最长回文子串|Medium|$O(n^2)$|字符串|No|从中心向两边遍历，动态规划|
|7.整数反转|Easy|$O(n)$|字符串|Done|直接翻转|
|8.字符串转换整数 (atoi)|Medium|$O(n)$|字符串|Done|主要是各种边界条件|
|9.回文数|Easy|$O(n)$|字符串|Done|翻转后判断是否相等|
|10.正则表达式匹配|Hard|   |字符串、递归|No|匹配符号|
|11.盛最多水的容器|Medium|$O(n)$|数组、双指针|Done|左右双指针谁小谁移动|
|13.罗马数字转整数|Easy|$O(n)$|数学、字符串|Done|注意需要正负号反转的这个数|
|14.最长公共前缀|Easy|$O(mn)$|字符串|No|水平或垂直比较|
|15.三数之和|Medium|$O(n^2)$|数组、双指针、哈希表|Done|排序然后双指针，哈希表判断|
|16.最接近的三个数之和|Medium|$O(n^2)$|双指针|No|同样是排序后双指针|
|17.电话号码的字母组合|Medium|$O(4^M*3^N)$|数组、回溯|No|每次对前面的字符串组成的字母组合进行遍历|
|19.删除链表的倒数第N个节点|Medium|$O(n)$|链表|Done|设置哑结点，快慢指针，遍历到第L-n个结点|
|20.有效的括号|Easy|$O(n)$|栈、字符串|Done|判断新符号和栈顶元素是否可消掉|
|21.合并两个有序链表|Easy|$O(m+n)$|链表|Done|递归不断接下一个较小结点|
|22.括号生成|Medium|$O(2^{2N}*N)$|字符串、回溯|No|左括号数小于n，右括号数小于左括号数|
|23.合并K个排序链表|Hard|$O(kN)$|链表、分置|No|归并；整个转换成list，排序，然后转变成链表|
|26.删除排序数组中的重复项|Easy|$O(n)$|数组、双指针|Done|双指针，第一个遍历，第二个保存有多少个重复元素|
|28.实现strStr()|Easy|$O(n)$|字符串|Done|滑窗遍历,KMP|
|29.两数相除|Meidum|  |数学|Done|模拟除法的原理|
|31.下一个排列|Medium|$O(n)$|数组|No|围绕满足nums[k] < nums[k+1]的最大索引|
|32.最长有效括号|Hard|$O(n^2)$|字符串|No|动态规划|
|34.在排序数组中查找元素的第一个和最后一个位置|Medium|$O(logn)$|二分查找|No|通过二分查找寻找左右边界|
|36.有效的数独|Medium|$O(1)$|哈希表、数组|Done|按照定义解决|
|39.组合总和|Medium|  |回溯|No|回溯法不断寻找，要固定一个模板|
|40.组合总和II|Medium| |回溯|No|后续数组，需要不断更新，去除已经选择的数|
|42.接雨水|Hard|$O(n)$|数组、双指针|No|寻找左右两边柱子最大高度的最小值|
|43.字符串相乘|Medium|$O(mn)$|字符串、数学|Done|转换成数字相乘、竖式|
|45.跳跃游戏II|Hard|$O(n)$|贪心，DP|No|dp[i] = max(dp[i], dp[j]+1) for j in [0,i-1] if nums[j] >= i-j|
|46.全排列|Medium|  |回溯|No|深刻理解回溯算法|
|47.全排列II|Medium|  |回溯|Done|和上述类似，每次添加的时候加一个判断|
|48.旋转图像|Medium|$O(n^2)$|数组|Done|先翻转（颠倒）然后转置|
|49.子母异位词分组|Medium|$O(nk)$|哈希表|No|将排序后字符串或统计次数作为key，相同的字符串保存对应key的list中|
|50.Pow(x,n)|Medium|$O(logn)$|二分查找|Done|递归求解，修改函数参数而不是对函数返回值累乘|
|53.最大子序列和|Easy|$O(n)$|数组、动态规划|Done|$f(n) = max(f(n-1)+nums[n], nums[n])$|
|54.螺旋矩阵|Medium|$O(mn)$|数组|No|方向数组，每次判断是否满足条件，转变方向，di+1，否则一直持续同一个方向|
|55.跳跃游戏|Medium|$O(n)$|贪心、数字|Done|每次获取当前步所能到达的最远距离|
|56.合并区间|Medium|$O(nlogn)$|排序、数组|No|按start排序，然后根据是否重叠拼接|
|59.螺旋矩阵II|Medium|$O(n^2)$|数组|Done|方向指针，主要是方向的判断，顺时针遍历|
|62.不同路径|Meidum|$O(1),O(mn)$|排列组合、动态规划|Done|状态方程为上边和左边的状态求和|
|63.不同路径II|Medium|$O(mn)$|动态规划|No|有障碍物的地方dp[i][j]为0|
|64.最小路径和|Medium|$O(mn)$|DP|Done|dp[i][j] = min(dp[i-1][j],dp[i][j-1]) + grid[i][j]|
|66.加一|Easy|$O(n)$|数学|Done|转换成字符串|
|69.x的平方根|Easy|$(logn)$|二分查找|No|关键是边界条件|
|70.爬楼梯|Easy|$O(n)$|数学|Done|斐波那契数列|
|72.编辑距离|Hard|$O(n^2)$|DP|No|dp[i][j] = min(dp[i-1][j-1], dp[i-1][j], dp[i][j-1]) + 1|
|74.搜索二维矩阵|Medium|$O(n)$|数组|Done|从右上遍历到左下|
|75.颜色分类|Medium|$O(m)$|排序|Done|遍历两次数组|
|76.最小覆盖子串|Hard|$O(m+n)$|滑窗法|No|移动左右窗口边界|
|77.组合|Medium| |回溯|Done|类似17题，套用回溯模板|
|78.子集|Medium| |回溯（递归）|No|依然是回溯的写法吧|
|79.单词搜索|Medium|  |回溯|No|遍历每一个点，然后将其作为字符串的起点进行回溯|
|84.柱状图中最大的矩形|Hard|$O(n)$|栈|No|每次用栈只保存递增序列|
|88.合并两个有序数组|Easy|$O(m+n)$|归并|Done|归并思想，依次选择较小的元素进行拼接|
|90.子集II|Medium|  |回溯|Done|回溯模板，判断重复，需要进行剪枝|
|92.反转链表II|Medium|$O(n)$|链表|No|首先结点移动到反转起始位置，然后反转链表，直到反转的截止处|
|94.二叉树的中序遍历|Medium|$O(n)$|树、DFS|Done|递归遍历，依次左根右|
|96.不同的二叉搜索树|Medium|$O(n)$|二叉树、DP，数学|No|$C_0 = 1,C_{n+1} = \frac{2(2n+1)}{n+2}C_n$|
|98.验证二叉搜索树|Medium|$O(n)$|树、DFS|No|中序遍历，判断是否满足递增序列|
|100.相同的树|Easy|$O(n)$|树、递归|Done|递归遍历判断每一个结点是否相同|
|101.对称二叉树|Easy|$O(n)$|二叉树|No|递归判断左右子树是否相等|
|102.二叉树的层次遍历|Medium|$O(n)$|二叉树、队列、BFS|Done|建立一个队列然后BFS遍历|
|103.二叉树的锯齿形层次遍历|Medium|$O(n)$|DFS、二叉树、队列|Done|相比上一题增加一个奇偶的判断|
|104.二叉树的最大深度|Easy|$O(n)$|二叉树、递归|Done|递归遍历结点，求左右子树的深度|
|105.从前序与中序遍历序列构造二叉树|Medium|$O(n)$|二叉树、递归，DFS|No|先获取根结点，然后对左右子树递归调用|
|106.从中序与后序遍历序列构造二叉树|Medium|$O(n)$|二叉树、递归，DFS|Done|同上，主要是中序遍历和后序遍历的识别|
|108.将有序数组转换为二叉搜索树|Medium|$O(n)$|二叉树、递归|Done|先得到根节点，然后左右子树遍历生成|
|110.平衡二叉树|Easy|$O(n^2)$|二叉树、递归，DFS|Done|判断每个结点左右子树的深度差是否小于1|
|112.路径总和|Easy|$O(n)$|二叉树、迭代、递归|No|遍历每一个结点，然后到叶节点判断sum|
|113.路径总和II|Medium|$O(n)$|二叉树、迭代、递归、树的遍历|No|主要是递归和迭代的套路是啥|
|114.二叉树展开为链表|Meidum|$O(n)$|二叉树、链表、DFS|No|关键是如何原地修改|
|118.杨辉三角|Easy|$O(n^2)$|数组|Done|根据上一层构建下一层，找到关系式即可|
|121.买卖股票的最佳时机|Easy|$O(n)$|数组|Done|两个变量，到目前为止的最小价格和最大利润|
|122.买卖股票的最佳时机II|Easy|$O(n)$|数组、贪心|Done|不断添加波谷波峰|
|123.买卖股票的最佳时机III|Medium|$O(n)$|动态规划|No|两次交易，分开简历状态转移方程|
|124.二叉树的最大路径和|Hard|$O(n)$|DFS|No|求每个结点作为根节点到叶节点的的最大路径和，不停更新全局变量|
|128.最长连续序列|Hard|$O(n)$|哈希表|No|将nums保存成set，如果num-1不在set中启动遍历|
|131.分割回文串|Medium|  |回溯|No|回溯法，s为空则保存，否则继续遍历，遍历所有头回文串|
|136.只出现一次的数字|Easy|$O(n)$|数组、哈希表、位运算|Done|统计次数、数学公式、异或|
|137.只出现一次的数字II|Easy|$O(n)$|数组、哈希表、位运算|Done|很迷，此处位运算麻烦些|
|139.单词拆分|Medium|$O(n^2)$|DP|Done|dp[i] = if dp[j] and s[j:i] in wordDict for j in range(0,i)|
|141.环形链表|Easy|$O(n)$|链表、双指针|Done|快慢指针或者设置特殊值然后判断|
|142.环形链表II|Medium|$O(n)$|链表，双指针，哈希表|Done|哈希表保存已知结点位置，判断新节点是否在哈希表中|
|144.二叉树的前序遍历|Easy|$O(n)$|二叉树、DFS|Done|递归遍历，根左右结点|
|145.二叉树的后序遍历|Medium|$O(n)$|二叉树、DFS|Done|递归遍历，左右跟结点|
|146.LRU缓存机制|Medium|$O(1)$|哈希表|No|使用有序字典来实现|
|148.排序链表|Medium|$O(nlogn)$|链表、排序|Done|先放在一个数组里面排序，然后重新生成链表|
|152.乘积最大子序列|Medium|$O(n^3)$|数组|No|$fmax(i) = max(fmax(i-1)*num[i], fmin(i-1)*num[i], num[i]),fmin(i) = min(fmax(i-1)*num[i], fmin(i-1)*num[i], num[i])$|
|153.寻找旋转排序数组中的最小值|Medium|$O(logn)$|数组，二分查找|Done|二分查找不断更新值|
|154.寻找旋转排序数组中的最小值 II|Hard|$O(logn)$|数组、二分查找|Done|和上述类似，只需考虑重复值|
|155.最小栈|Easy|$O(1)$|栈|Done|建立辅助栈,每次保存新元素和已知元素|
|160.相交链表|Easy|$O(m+n)$|链表|Done|长链表先走，然后再一起走|
|167.两数之和 II-输入有序数组|Easy|$O(n)$|数组、双指针、二分查找|Done|双指针，前后遍历|
|169.求众数|Easy|$O(n)$|数组、哈希表|Done|哈希表(统计次数)|
|171.Excel表列序号|Easy|$O(n)$|数学|Done|模拟进制转换|
|172.阶乘后的零|Easy|$O(logn)$|数学|No|求每一部分因子为5的个数|
|179.最大数|Medium||数组、排序|No|关键是排序规则书写，熟悉key和cmp_to_key|
|189.旋转数组|Easy|$O(1)$|数组|Done|注意原地操作|
|191.位1的个数|Easy|$O(n)$|位运算|Done|统计1的个数即可|
|198.打家劫舍|Easy|$O(n)$|动态规划|No|$f(n) = max(f(n-1), f(n-2)+nums[n])$|
|200.岛屿数量|Medium|$O(mn)$|dfs|No|遍历每一个点，令1周围的1都变成0|
|201.数字范围按位与|Easy|$O(n)$|位运算|No|发现二进制的规律|
|202.快乐数|Easy|  |哈希表、数组|No|1-4之间只有1是快乐数，>4的非快乐数都会进入4或者3的循环序列|
|204.计算质数|Easy|$O(n)$|哈希表、数学|No|设置质数数组，然后让质数的倍数为False|
|206.反转链表|Easy|$O(n)$|链表|Done|依次翻转|
|207.课程表|Medium|$O(E+V)$|图|No|拓扑排序|
|208.前缀树|Medium|$O(n)$|二叉树|No|字典实现这种数据结构|
|215.数组中的第K个最大的元素|Medium|$O(n)$|数组、堆|Done|利用最小堆实现|
|216.组合总和III|Medium|$O(n)$|回溯|Done|回溯，加一个判断，判断长度|
|217.存在重复元素|Easy|$O(n)$|哈希表|Done|哈希表判断|
|219.存在重复元素II|Easy|$O(n)|哈希表|Done|哈希表保存每个数出现的位置，增加一个条件判断索引|
|220.存在重复元素III|Medium|$O(n)$|桶排序|No|复杂度达不到要求|
|221.最大正方形|Medium|$O(mn)$|DP|No|dp[i][j] = min(dp[i-1][j],dp[i][j-1],dp[i-1][j-1]) + 1|
|225.用队列实现栈|Easy|  |队列、栈|
|226.翻转二叉树|Easy|$O(n)$|二叉树、递归|Done|递归翻转|
|229.求众数II|Medium|$O(n)$|数组、排序、哈希表|Done|哈希表统计次数|
|230.二叉搜索树中第k小的元素|Medium|$O(n)$|二叉树、dfs|Done|中序遍历，得到排序数组|
|231.2的幂|Easy|$log(n)$|数学|Done|依次除以2，直到不能整除，判断最后是否是1|
|232.用栈实现队列|Easy||栈、队列|Done|建立一个辅助栈，模拟倒水的过程|
|234.回文链表|Easy|$O(n)$|链表、指针|Done|转成数组然后判断是否是回文数组|
|235.二叉搜索树的最低公共祖先|Easy|$O(n)$|二叉树、dfs|No|判断p，q是否在根节点和左右子树出现过|
|236.二叉树的最低公共祖先|Medium|$O(n)$|二叉树，dfs|No|求以node为根结点的子树是否出现过两个结点|
|237.删除链表中的结点|Easy|$O(1)$|链表|Done|val和next分别赋值|
|238.除自身以外数组的乘积|Medium|$O(n)$|数组|Done|左右分别累乘，注意边界值|
|239.滑动窗口最大值|Hard|$O(n)$|数组、堆、队列|No|最优解不会|
|240.搜索二维矩阵II|Medium|$O(m+n)$|数组、二分查找|Done|从左上遍历到右下|
|242.有效的字母异位词|Easy|$O(n)$|哈希表|Done|Counter统计每个字符的次数|
|260.只出现一次的数字III|Medium|$O(n)$|数组、哈希表|Done|我佛|
|268.缺失数字|Easy|$O(n)$|数学|Done|公式求解|
|279.完全平方数|Medium|$O(n)$|数学、DP|No|动态规划超时，数学方法最优|
|283.移动零|Easy|$O(n)$|数组、双指针|Done|移除0，然后append0|
|287.寻找重复数|Medium|$O(n),O(nlogn)$|二分法、链表|No|同时满足多个条件比较麻烦|
|289.生命游戏|Medium|$O(mn)$|数组|Done|按照题意遍历既可以，每次判断|
|292.Nim游戏|Easy|$O(1)$|数学|Done|如果是4的倍数肯定会输|
|295.数据流中的中位数|Hard|$O(n)$|最小堆，二分|No|二分插入排序，优先队列，双堆|
|300.最长上升子序列|Medium|$O(logn)$|数组、贪心、DP|No|依次添加比较小的数在辅助序列里面|
|309.最佳买卖股票时机含冷冻期|Medium|$O(n)$|动态规划|No|状态转移方程|
|312.戳气球|Hard|$O(n^3)$|DP|No|dp[i][j] = max(nums[i]*nums[k] *nums[j]+dp[i][k]+dp[k][j])|
|315.计算右侧小于当前元素的个数|Medium|$O(n)$|数组|No|。。。|
|322.零钱兑换|Medium|$O(Sn)$|动态规划|No|dp[i] = min(dp[i], dp[i-coin]+1) for coin in coins|
|326.3的幂|Easy|$O(log(n))$|数学|Done|循环遍历|
|328.奇偶链表|Medium|$O(n)$|链表|No|奇偶位置，分开保存在两个链表中|
|334.递增的三元子序列|Medium|$O(n)$|数组|Done|三元组判断|
|337.打家劫舍III|Medium|  |动态规划、二叉树|No|一个二元数组代表是否包含根节点|
|338.比特位计数|Medium|$O(32n)$|二进制|Done|和191类似，无差别|
|344.反转字符串|Easy|$O(n)$|字符串|Done|原地翻转|
|347.前 K 个高频元素|Medium|$O(n)$|堆、哈希表|No|和215类似，但需要注意更多的地方|
|350.两个数组的交集II|Easy|$O(m,n)$|数组、哈希表|Done|Counter转成字典判断，排序后比较|
|371.两整数之和|Easy|$O(n)$|位运算|No|异或代表求和，与代表进位，二进制来求解|
|384.打乱数组|Medium|$O(n)$|数组|Done|做拷贝，利用random.shuffle打乱|
|387.字符串中的第一个唯一字符|Easy|$O(n)$|哈希表|Done|直接统计次数即可|
|392.判断子序列|Easy|$O(n)$|队列|Done|判断目标字符串，如果能匹配，则删除第一个字符|
|394.字符串解码|Medium|$O(n)$|栈|No|‘[’：括号外的字符串和出现次数入栈，']'：括号内的字符串出栈|
|395.至少有k个重复字符的最长子串|Medium|  |递归、分治|No|对原始字符串进行拆解，然后递归调用|
|399.除法求值|Medium|$O(n)$|图、DFS|No|转换成图，然后利用图结构求解|
|406.根据身高重建队列|Medium|$O(nlogn)$|数组、排序|No|对身高降序排序，人数升序排序|
|410.分割数组的最大值|Hard|$O(nlog(sum/k))$|二分查找、贪心|No|遍历值，判断和是否存在|
|412.Fizz Buzz|Easy|$O(n)$|数学|Done|直接遍历|
|416.分割等和子集|Medium|$O(ns)$|DP|No|dp[i][j] = dp[i-1][j] or dp[i-1][j-nums[i]],(nums[i] <= j)|
|414.第三大的数|Easy|$O(n)$|数组、堆|Done|和215类似，同时可以用规则|
|437.路径总和III|Easy|$O(n)$|树、栈、递归|No|对题意的理解以及对树深度遍历的把控|
|438.找到字符串中所有字母异位词|Easy|$O(n)$|哈希表、滑窗法|No|滑窗法，不断移动左右边界来判断| 
|448.找到所有数组中消失的数字|Easy|$O(n)$|数组、哈希表|Done|遍历，然后判断，按索引求反|
|461.汉明距离|Easy|$O(n)$|位运算|Done|做异或，然后统计1的个数|
|477.汉明距离总和|Medium|$O(36*n)$|位运算|No|不可两两异或，求每一位1的个数和0的个数，然后相乘求和|
|494.目标和|Medium|$O(n^2)$|背包问题|No|不懂，不会|
|496.下一个更大的元素I|Easy|$O(n)$|栈、哈希表|Done|类似739题，都是相似的|
|503.下一个更大的元素II|Medium|$O(n)$|栈|Done|和496类似，对nums做一个复制|
|523.连续的子数组和|Medium|$O(n^2)$|数组|Done|和560相似，求子数组和即可|
|538.把二叉搜索树转换为累加树|Medium|  |二叉树、递归|No|反向中序遍历，先右子树，然后根节点累加，然后左子树|
|543.二叉树的直径|Easy|$O(n)$|二叉树、DFS|No|和求树的深度一样，路径为L+R+1|
|557.翻转字符串中的单词III|Easy|$O(n)$|字符串|Done|空格划分，然后单词内翻转|
|560.和为K的子数组|Medium|$O(n)$|哈希表、数组|No|保存累积求和出现的次数|
|581.最短无序连续子数组|Easy|$O(nlogn)$|数组、排序、栈|Done|先排序，然后比较不同元素的索引|
|617.合并二叉树|Easy|$O(n)$|二叉树、递归|Done|对每个子节点递归，判断根节点是否为空| 
|647.回文子串|Medium|$O(n^2)$|字符串|Done|中心扩散|
|654.最大二叉树|Medium|    |二叉树、递归|Done|对整个数组和左右边数组依次递归调用|
|668.乘法表中的第k小的数|Hard|$O(mlog(mn))$|二分查找|No|太难了不会|
|704.二分查找|Easy|$O(logn)$|二分查找|Done|直接上模板|
|714.买卖股票的最佳时机含手续费|Medium|$O(n)$|数组、动态规划|Done|和122类似，弄懂122|
|739.每日温度|Medium|$O(n)$|栈|No|根据温度大小关系，不断将其入栈|
|746.使用最小花费爬楼梯|Easy|$O(n)$|DP|Done|dp[i] = min(dp[i-1],dp[i-2]) + cost[i]|
|876.链表的中间结点|Easy|$O(n)$|链表，双指针|Done|快慢指针|
|1047.删除字符串中的所有相邻重复项|Medium|$O(n)$|栈、字符串|Done|新元素和栈顶元素比较|