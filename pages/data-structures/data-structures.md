---
layout: default
title: Data Structures
permalink: /data-structures
nav_order: 3
has_children: true
has_toc: true
---

<h1>Data Structures</h1>
### Introduction
<p>
  <i>What is a Data Structures?</i>
</p>
<p class="concept l-font">
  A Data Structure is a particular way of organizing information on a computer so that it
  can be used efficiently. Different types of data structures are suitable
  for <b>different</b> types of applications, and some are <b>highly specialized</b> for specific tasks.
</p>
<p class="l-font">
  The data structures are used to make different solutions for computacional problems that may involve
  complex process such as large databases and Internet indexing services.
  <br><br>
  Since I work with Java and JavaScript I will explain the implementation in these languages.
</p>

## Java implementation
<p class="l-font">
  Java has a framework for implementing data structures,
  it is called the <code class="fs-3"><b>Java Collections Framework</b></code>. I <b>highly recommend</b> reviewing the
  official
  documentation for this framework on the <a
    href="https://docs.oracle.com/javase/8/docs/technotes/guides/collections/overview.html" target="_blank">Java
    API</a>.
</p>
<p class="l-font">
  Java Collections Framework is a combination of <code>classes</code> and <code>interfaces</code>, which is used to
  <b>store and manipulate</b>
  the data in the form of objects. First of all, let's list all the content it offers:
</p>
<div style="text-align: center;"><img src="{{ site.url }}{% link /assets/images/data-structures/java-collection-graph.png %}" alt=""
    style="border-radius: 6px">
</div>
<p class="important fs-5">
  It is important to highlight how the <b><u>Map interface</u></b> is part of the Collection framework <strong>BUT</strong> 
  <b><u>does not inherit</u></b> from the <b><u>Collection interface</u></b>. <span class="fs-3">*if concepts like 
    <i>"inherits"</i>, <i>"interfaces"</i> or <i>"classes"</i> don't sound familiar, first check out my page of <a href="{{ site.url }}{% link pages/oop/oop.md %}">Object Oriented Programming</a>.</span>
</p>
<p class="l-font">
  At first glance it may seem complicated to understand the graph, but let's order the data:
</p>
<table>
  <tr>
    <td class="v-align-top" style="text-align: center;" width="50%">
      <span class="fs-6"><b>Interfaces</b></span>
    </td>
    <td class="v-align-top" style="text-align: center;" width="50%">
      <span class="fs-6"><b>Classes</b></span>
    </td>
  </tr>
  <tr>
    <td class="v-align-top" width="50%">
      <ol class="ml-3">
        <li>Iterable</li>
        <li>Collection</li>
        <li>List</li>
        <li>Queue</li>
        <li>Set</li>
        <li>Dequeue</li>
        <li>SortedSet</li>
        <li>Map</li>
        <li>SortedMap</li>
      </ol>
    </td>
    <td class="v-align-top" width="50%">
      <ol class="ml-3">
        <li>ArrayList</li>
        <li>LinkedList</li>
        <li>Vector</li>
        <li>Stack</li>
        <li>Priority Queue</li>
        <li>ArrayDequeue</li>
        <li>HashSet</li>
        <li>LinkedHashSet</li>
        <li>TreeSet</li>
        <li>HashTable</li>
        <li>LinkedHashMap</li>
        <li>HashMap</li>
        <li>TreeMap</li>
      </ol>
    </td>
  </tr>
</table>
<p>
  Every Class has very specific functions, so 
  visit the corresponding page to know more about it.
</p>