学习笔记
// 递归代码模板Java
public void recur(int level, int param) { 
  // terminator 
  if (level > MAX_LEVEL) { 
    // process result 
    return; 
  }
  // process current logic 
  process(level, param); 
  // drill down 
  recur( level: level + 1, newParam); 
  // restore current status 
 
}


//分治代码模板Java
private static int divide_conquer(Problem problem, ) {
  
  if (problem == NULL) {
    int res = process_last_result();
    return res;     
  }
  subProblems = split_problem(problem)
  
  res0 = divide_conquer(subProblems[0])
  res1 = divide_conquer(subProblems[1])
  
  result = process_result(res0, res1);
  
  return result;
}

//动态规划关键点
1.最优子结构opt[n]=best_of(opt[n-1],opt[n-2],...)
2.储存中间状态：opt[i]
3.递推公式（美其名曰：状态转移方程或者DP方程）
Fib:opt[i]=opt[n-1]+opt[n-2]
二维路径：opt[i,j]=opt[i+1][j]+opt[i][j+1](且判断a[i,j]是否空地）

动态规划小结：
1.打破自己的思维惯性，形成机器思维
2.理解复杂逻辑的关键
3.也是职业进阶的的要点要领