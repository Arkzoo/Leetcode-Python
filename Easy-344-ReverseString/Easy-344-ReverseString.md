##ReverseString##
Leetcode链接：[ReverseString](https://leetcode.com/problems/reverse-string/)
##我自己的方法###
<pre><code>class Solution(object):
	def reverseString(self, s):
		"""
		:type s: str
		:rtype: str
		"""
		rs = ""
		for i in range(1,len(s)):
			rs = rs + s[-i]
		return rs </code></pre>
sub后结果是TLE。我自己用IDE测试没有问题（没有测时间）。不明白Leetcode的时间要求。**没弄明白**
##其他人的方法##
###Extended Slicing
>In  Python  2.3  and  later,  slice  expressions  have  support  for  an  optional  third  index,  used as  a  step  (sometimes  called  a  stride).  The  step  is  added  to  the  index  of  each  item  extracted.  The  full-blown  form  of  a  slice  is  now  X[I:J:K],  which  means  “extract  all  the items  in  X,  from  offset  I  through  J−1,  by  K.”  The  third  limit,  K,  defaults  to  +1,  which  is why normally all  items  in  a  slice  are  extracted  from  left  to  right.  If  you  specify  an  explicit value, however, you can use the third limit to skip items or to reverse their order. 

     
		
