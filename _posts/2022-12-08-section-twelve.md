---
keywords: fastai
summary: Sections 12 and 13 of big idea 3
title: Section 12 and 13
toc: true
layout: post
description: Big Idea 3 sections 12 and 13
categories: [week-14]
author: Aditya Ajay Nawandhar
show_tags: true
comments: true
image: images/postimage6.png
nb_path: _notebooks/2022-12-08-section-twelve.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-12-08-section-twelve.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Notes:">Notes:<a class="anchor-link" href="#Notes:"> </a></h2><ul>
<li>to creat a unique function in javasctript we use function as opposed to def in python.</li>
<li>Procedure:is a named group of programming instructions that may have parameters and return values.</li>
<li>Parameters:are input values of a procedure.</li>
<li>Arguments: specify the values of the parameters when a procedure is called</li>
<li>Modularity:Separating a program's functions into independent pieces or blocks, each containing all the parts needed to execute a single aspect of the functionality is called modularity</li>
<li>Procedural Abstraction: provides a name for a process that allows a procedure to be used only knowing WHAT it does, not HOW it does it</li>
<li>What are some other names for procedures?: can be anything that you want, </li>
<li>Why are procedures effective? We have the ability to alter the result without actually changing the calls to the program; Convenient to change the actions if there is an error in the code; able to break the code up and abstract what different part of the code does; helps identiy bugs, error</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="challnge-1">challnge 1<a class="anchor-link" href="#challnge-1"> </a></h3>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">function</span> <span class="n">convert</span><span class="p">(</span><span class="n">inti</span><span class="p">)</span>
    <span class="k">return</span> <span class="p">(</span><span class="n">inti</span><span class="p">)</span><span class="o">.</span><span class="n">toString</span><span class="p">(</span><span class="mi">2</span><span class="p">)</span>

<span class="n">decimal</span> <span class="o">=</span> <span class="mi">7</span>
<span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="n">convert</span><span class="p">(</span><span class="n">decimal</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_text output_error">
<pre>
<span class="ansi-cyan-fg">  Input </span><span class="ansi-green-fg">In [2]</span>
<span class="ansi-red-fg">    function convert(inti) {</span>
             ^
<span class="ansi-red-fg">SyntaxError</span><span class="ansi-red-fg">:</span> invalid syntax
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Challege-2">Challege 2<a class="anchor-link" href="#Challege-2"> </a></h3>
</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">findmax</span><span class="p">(</span><span class="n">a</span><span class="p">,</span> <span class="n">b</span><span class="p">):</span>
    <span class="k">if</span> <span class="n">a</span> <span class="o">&gt;</span> <span class="n">b</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">a</span><span class="p">)</span>
    <span class="k">elif</span> <span class="n">b</span> <span class="o">&gt;</span> <span class="n">a</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">b</span><span class="p">)</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;they are equal&quot;</span><span class="p">)</span>
        
<span class="k">def</span> <span class="nf">findmin</span><span class="p">(</span><span class="n">c</span><span class="p">,</span> <span class="n">d</span><span class="p">):</span>
    <span class="k">if</span> <span class="n">c</span> <span class="o">&lt;</span> <span class="n">d</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">c</span><span class="p">)</span>
    <span class="k">elif</span> <span class="n">c</span> <span class="o">&lt;</span> <span class="n">d</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">d</span><span class="p">)</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;they are equal&quot;</span><span class="p">)</span>
        

<span class="nb">print</span><span class="p">(</span><span class="n">findmax</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="n">findmin</span><span class="p">(</span><span class="mi">4</span><span class="p">,</span><span class="mi">5</span><span class="p">))</span>
        
<span class="c1"># Within the procedure, write the code to determine which of the two parameters, numberA or numberB, is the larger value. Print that value.</span>

<span class="c1"># Repeat the process, this time creating a procedure called findMin, which will print the parameter with a smaller value.</span>

<span class="c1"># Call both functions so that the parameters numberA and numberB are given a value.</span>

<span class="c1"># Optional bonus- create a procedure that can determine the minimum or maximum value out of more than two parameters.</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>3
None
4
None
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">function</span> <span class="n">findmax</span><span class="p">(</span><span class="n">numberA</span><span class="p">,</span> <span class="n">numberb</span><span class="p">){</span>
    <span class="k">if</span><span class="p">(</span><span class="n">numberA</span> <span class="o">&gt;</span> <span class="n">numberb</span><span class="p">){</span>
        <span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="n">numberA</span><span class="p">)</span>
    <span class="p">}</span>
    <span class="k">else</span> <span class="p">{</span>
        <span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="n">numberb</span><span class="p">)</span>
    <span class="p">}</span>
<span class="p">}</span>

<span class="n">function</span> <span class="n">findmin</span><span class="p">(</span><span class="n">numberA</span><span class="p">,</span> <span class="n">numberb</span><span class="p">){</span>
    <span class="k">if</span><span class="p">(</span><span class="n">numberA</span> <span class="o">&lt;</span> <span class="n">numberb</span><span class="p">){</span>
        <span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="n">numberA</span><span class="p">)</span>
    <span class="p">}</span>
    <span class="k">else</span> <span class="p">{</span>
        <span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="n">numberb</span><span class="p">)</span>
    <span class="p">}</span>
<span class="p">}</span>

<span class="n">findmax</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
<span class="n">findmin</span><span class="p">(</span><span class="mi">4</span><span class="p">,</span> <span class="mi">5</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>3
4
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Homework">Homework<a class="anchor-link" href="#Homework"> </a></h2><ul>
<li>One way we can do it is by using the ord function to convert every letter in the string APCSP into their corresponding number using ord() function which returns the unicode for a specified character. </li>
<li>then using the bin() function that converts number to binary and print that.</li>
<li>I did the same code in 2 ways, one way is using bytearray and for loop while the other method is using the ord() function and the bin() function to make the string to a unicode value and use that integer value into binary.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">str</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;any word or sentence: &quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The original string is : &quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">)</span>

<span class="n">result</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">format</span><span class="p">(</span><span class="n">i</span><span class="p">,</span> <span class="s1">&#39;08b&#39;</span><span class="p">)</span> <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">bytearray</span><span class="p">(</span><span class="nb">str</span><span class="p">,</span> <span class="n">encoding</span> <span class="o">=</span><span class="s1">&#39;utf-8&#39;</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;The string after binary conversion : &quot;</span><span class="p">,</span> <span class="n">result</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>The original string is :  APCSP
The string after binary conversion :  0100000101010000010000110101001101010000
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">converter</span><span class="p">(</span><span class="n">islow</span><span class="p">):</span>
    <span class="n">new_list</span> <span class="o">=</span> <span class="p">[]</span>
    <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">input_str</span><span class="p">:</span>
        <span class="n">p</span> <span class="o">=</span> <span class="nb">ord</span><span class="p">(</span><span class="n">i</span><span class="p">)</span>
        <span class="n">new_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="nb">bin</span><span class="p">(</span><span class="n">p</span><span class="p">)</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;0b&quot;</span><span class="p">,</span> <span class="s2">&quot;&quot;</span><span class="p">))</span>
    
    <span class="n">new</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
    <span class="n">values</span> <span class="o">=</span> <span class="n">new</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">new_list</span><span class="p">)</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;the input value is: &quot;</span><span class="p">,</span> <span class="n">islow</span><span class="p">)</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">values</span><span class="p">)</span>
    <span class="k">return</span> <span class="n">new_list</span>
    


<span class="n">input_str</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;any word: &quot;</span><span class="p">)</span>
<span class="nb">print</span><span class="p">(</span><span class="n">converter</span><span class="p">(</span><span class="n">input_str</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>the input value is:  APCSP
10000011010000100001110100111010000
[&#39;1000001&#39;, &#39;1010000&#39;, &#39;1000011&#39;, &#39;1010011&#39;, &#39;1010000&#39;]
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

