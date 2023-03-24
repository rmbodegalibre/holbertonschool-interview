<h1>Pascal's Triangle</h1>
<div class="panel-heading panel-heading-actions">
<h3 class="panel-title">0. Pascal's Triangle</h3>
<div><span class="label label-info">mandatory</span></div>
</div>
<div class="panel-body"><span id="user_id" data-id="4578"></span>
<p>Create a function&nbsp;<code>def pascal_triangle(n):</code>&nbsp;that returns a list of lists of integers representing the Pascal&rsquo;s triangle of&nbsp;<code>n</code>:</p>
<ul>
<li>Returns an empty list if&nbsp;<code>n &lt;= 0</code></li>
<li>You can assume&nbsp;<code>n</code>&nbsp;will be always an integer</li>
</ul>
</div>
<pre><code>guillaume@ubuntu:~/$ cat 0-main.py
#!/usr/bin/python3
"""
0-main
"""
pascal_triangle = __import__('0-pascal_triangle').pascal_triangle

def print_triangle(triangle):
    """
    Print the triangle
    """
    for row in triangle:
        print("[{}]".format(",".join([str(x) for x in row])))


if __name__ == "__main__":
    print_triangle(pascal_triangle(5))

guillaume@ubuntu:~/$ 
guillaume@ubuntu:~/$ ./0-main.py
[1]
[1,1]
[1,2,1]
[1,3,3,1]
[1,4,6,4,1]
guillaume@ubuntu:~/$ </code></pre>