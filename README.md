# ustc-sse-thesis-latex
中国科学技术大学软件学院 硕士论文latex模板

此模板是作者自己使用的，仅供参考。

### 使用说明
#### 三线表
``
如\ref{tab:xx表}所示，xxx...
``

``
\begin{table}[h!]
  \renewcommand{\arraystretch}{1.5}
  \centering
  \caption{xx表}
  \begin{tabular}{cm{5cm}} % l, c, r 分别表示列的对齐方式：左对齐、居中、右对齐
    \toprule
    xx & xx  \\
    \midrule
    xx & xx \\
    \bottomrule
  \end{tabular}
  \label{tab:xx表}
\end{table}
``
- 1.5是字体和上下边界的距离
- `m{5cm}`表示该列内容垂直居中并且最大长度为5cm，超出内容会换行

#### 代码引用
``\begin{lstlisting}
func main(){
    fmt.Println("hello")
}
\end{lstlisting}``

代码块引用样式在ustcsetup.tex的\usepackage{listings}下面设置

#### 注意项
latex中的双引号应该是 ``内容" 的形式

## 撰写流程建议
个人建议流程：
1. 用markdown格式完成各个模块文字内容
2. 将markdown格式转换为tex格式
3. 使用在线编辑器编译，进行内容的排版
4. 导出文件

**上述流程都使用git进行版本管理**

## 相关资源
- [毕业论文流程攻略](https://www.wolai.com/xiaomingstudent/6fxAUz2KqaxWtjWWWmGKsd)

- 在线latex编辑器：[中科大Latex平台](https://latex.ustc.edu.cn/project) [overleaf](https://www.overleaf.com/project)

- [研究生学位论文撰写手册](./研究生学位论文撰写手册.pdf)