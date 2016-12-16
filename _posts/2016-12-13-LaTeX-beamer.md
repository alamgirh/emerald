---
layout: post
title: $\LaTeX$ ব্যবহার করে প্রেজেন্টেশন তৈরি 
date: 2016-12-13
categories: update
---

<img src="http://i.stack.imgur.com/zHFFO.png" class="fit image"> 

<p> প্রথমে একটি গল্প দিয়ে শুরু করি। এটি আমার গল্প। 2007 সালে আমি মাস্টার্সে পড়ি। তখন ঢাকা বিশ্ববিদ্যালয়ে বাংলাদেশ গণিত সমিতির কনফারেন্স অনুষ্ঠিত হয়। একটা কনফারেন্স কক্ষে আমি প্রেসেন্টারদের সাহায্য করছিলাম। কম্পিউটারে লেফট রাইট কী চেপে তাদের স্লাইড সরানোর কাজ। তার মধ্যে একটা প্রেজেন্টেশনের স্লাইড গুলো দেখে আমার খুব ভালো লাগে। এটি ছিল সিঙ্গাপুরের একজন বাংলাদেশী প্রফেসরের স্লাইডস। আমি ভাবতে থাকি কিভাবে এই ধরণের প্রেজেন্টেশন করা যায়। তখন আমি পাওয়ার পয়েন্ট ব্যবহার করে প্রেসেন্টেশন করতাম। পাওয়ার পয়েন্টের স্লাইড গুলোকে পিডিফ করে দেখলাম, মাইক্রোসফট ওয়ার্ডের ফাইলকে ল্যান্ডস্কেপ সেটিংস দিয়ে চেষ্টা করলাম তাতে ও ঐ রকম স্লাইডস বানাতে পারলাম না। তারপর বুঝতে পারলাম এটা অন্য কোনো সফ্টওয়ার বা পদ্ধতি যেটা আমাকে শিখতে হবে। 2013 সালে কানাডাতে এসে আমি সেই ফরম্যাটের প্রেজেন্টেশন ফাইল তৈরি করলাম। </p>

<p>আমি জানি পৃথিবীতে লক্ষ কোটি জিনিষ রয়েছে তার কতগুলো আমি শিখবো? কিন্তু গণিতের ছাত্র হিসেবে $\LaTeX$ ব্যবহার করে ডকুমেন্ট লিখা , সিভি তৈরি কিংবা প্রজেক্ট বা থিসিস অবশই লিখতে হবে। আমি নিজে নিজে লজ্জিত হই এই ভেবে যে $\LaTeX$ এর মতো একটা জিনিস আমাকে কানাডাতে এসে শিখতে হলো। হয়তো বাংলাদেশে থাকলে আমার কখনোই শেখা হতো না! </p>

<p>এখন মূল বক্তব্যে আসি। </p> 

<h2> কিভাবে $\LaTeX$ ব্যবহার করে প্রেজেন্টেশন স্লাইডস তৈরি করবেন?</h2>

<p> আপনার কম্পিউটারে আপনাকে একটি $\LaTeX$ সফ্টওয়ার ইনস্টল করতে হবে। যেমন <a href='http://www.xm1math.net/texmaker/'>Texmaker</a>, <a href='http://kile.sourceforge.net/'> Kile</a>  ইত্যাদি । এছাড়া অনলাইনে $\LaTeX$ ব্যবহারের জন্য <a href='https://www.sharelatex.com/'> sharelatex </a> এ একাউন্ট ওপেন করতে পারেন।  <a href='https://www.sharelatex.com/'> sharelatex </a> ব্যবহার করতে পারেন । সেখানে রয়েছে অসংখ্য <a href='https://www.sharelatex.com/templates/presentations'>প্রেজেন্টেশন Template</a>. আমি এই টিউটোরিয়ালটি প্রস্তুতির জন্য <a href='https://www.sharelatex.com/templates/presentations/conference-presentation'>conference-presentation</a> টেম্পলেটটি  ব্যবহার করেছি. </p>

<p> এছাড়া <a href='https://github.com/'> github </a> এ একাউন্ট খুলতে পারেন। <a href='https://github.com/'> github </a>  এ আপনি অসংখ্য প্রেজেন্টেশন Template খুঁজে পেতে পারেন। </p>

<h2> প্রেজেন্টেশন প্রস্তুতিতে ব্যবরিত .tex ফাইলের বিবরণ </h2>

<h3> Document Class </h3>
প্রেজেন্টেশন ফাইল প্রস্তুতির জন্য আপনার ডকুমেন্ট ক্লাস হবে beamer
```LaTeX
\documentclass{beamer}
```

<h3>Theme</h3> 

<p>অসংখ্য থিম রয়েছে। নিচে থিম গুলোর নাম উল্লেখ করেছি। এর মধ্যে থেকে আপনার পছন্দের থিম বাছাই করে নিতে পারেন।</p>

<p>AnnArbor, Antibes, Bergen, Berkeley, Berlin, Boadilla, boxes, CambridgeUS, Copenhagen, Darmstadt, default, Frankfurt,
Goettingen, Hannover, Ilmenau, JuanLesPins, Luebeck, Madrid,Malmoe, Marburg, Montpellier, PaloAlto, Pittsburgh, Rochester, Singapore, Szeged, Warsaw</p>
```LaTeX
\usetheme{CambridgeUS}
```
<h3>Frame</h3>
<p>ধরুন Quadratic Equation সম্পর্কে আপনি নিচের লেখা গুলো দুইটি স্লাইডে দেখতে দেখাতে চান.</p><br>
<p>When $a \ne 0$, quadratic equation $ax^2 + bx + c = 0$ has two roots and they are
$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$ 

$$ \begin{array}{rcl}
y & = & a x^{2}+bx+c\\
  & = & a\left(x^{2}+2\times\frac{b}{2a}x+\frac{c}{a}\right)\\
  & = & a\left(x+\frac{b}{2a}\right)^2 - \frac{b^2}{4a} + c
\end{array}$$

Vertex of the parabola, $y = f(x)$ is $\left(-\frac{b}{2a}, c - \frac{b^2}{4a}\right)$.</p>

<p>তাহলে লেখাটিকে আপনার .tex ফাইলে নিচের মত করে লিখে স্লাইড তৈরী করতে পারেন।</p>

```LaTeX
\begin{frame}
  \frametitle{Quadratic Equations}
    When $a \ne 0$, quadratic equation
    $$ ax^2 + bx + c = 0 $$ has two roots and they are
    $$x = \frac{-b \pm \sqrt{b^2-4ac}}{2a}.$$
\end{frame}

\begin{frame}
  \frametitle{Vertex of Parabola}
  \[ \begin{array}{rcl}
    y & = & a x^{2}+bx+c\\
      & = & a\left(x^{2}+2\times\frac{b}{2a}x+\frac{c}{a}\right)\\
      & = & a\left(x+\frac{b}{2a}\right)^2 - \frac{b^2}{4a} + c
  \end{array}\]
  Vertex of the parabola, $y = f(x)$ is
  $\left(-\frac{b}{2a}, c - \frac{b^2}{4a}\right)$.
\end{frame}
```

<a href='http://mathurl.com/'>mathURL</a> ব্যবহার করে গাণিতিক যেকোন লেখা বা সমীকরণ লিখতে পারেন। 

<h3> Block</h3>

```LaTeX
\begin{block}{Discriminant}
    $$d = b^2-4ac$$
\end{block}
```

<h3>Table</h3>

<a>এখন আপনি যদি নিচের মতো করে একটি টেবিল প্রস্তুত করতে চান:</a>

<table border="1">
<thead><tr>
<th>$d = b^2-4ac$</th>
<th>comment about roots</th>
</tr>
</thead>
<tbody>
<tr>
<td>$d>0$</td>
<td>roots are real and distinct</td>
</tr>
<tr>
<td>$d = 0$</td>
<td>roots are real and same</td>
</tr>
<tr>
<td> $d < 0$ </td>
<td>roots are complex</td>
</tr>
</tbody>
 </table>

তাহলে আপনার .tex ফাইলে নিচের মত করে লিখে একটি স্লাইড তৈরী করতে পারেন।

```LaTeX
\begin{frame}
  \frametitle{Table: Type of roots}
  \begin{center}
    \begin{tabular}{|l|l|}
      \hline
      $d = b^2-4ac$ & comment about roots\\
      \hline \hline
      $d>0$ & roots are real and distinct\\
      \hline
      $d = 0$ & roots are real and same\\
      \hline
      $d<0$ & roots are complex\\
      \hline
    \end{tabular}
  \end{center}
\end{frame}
```

<h3> Figure </h3>

এখন আপনার আগ্রহ তৈরি হতে পারে আপনার প্রেসেন্টেশন ফাইলে একটি ছবি সংযুক্ত করবেন। যেমন quadraticplots.png ফাইল আপনি সংযুক্ত করতে চান। 

<img src="https://alamgirh.github.io/tutorial/latex-presentation-tutorial/quadraticplots.png" class="fit image"> 

তাহলে আপনার .tex ফাইলে নিচের মত করে লিখে একটি স্লাইড তৈরী করতে পারেন।

```LaTeX
\begin{frame}
  \frametitle{Plots of quadratic equations}
    \begin{figure}
    \centering
    \includegraphics[scale=0.5]{quadraticplots.png}
    \caption{LaTex: Quadratic Functions}
    \end{figure}
\end{frame}
```
<h3> ডাউনলোড লিংক</h3>
এই টিউটোরিয়ালে ব্যবহৃত .tex, .bib ফাইল ও $\LaTeX$ ব্যবহার করে প্রাপ্ত .pdf ফাইলের ডাউনলোড লিংক:
<ul>
<li> <a href='https://alamgirh.github.io/tutorial/latex-presentation-tutorial/QuadraticEquations.tex'>QuadraticEquations.tex</a></li>
<li> <a href='https://alamgirh.github.io/tutorial/latex-presentation-tutorial/QuadraticEquations.pdf'>QuadraticEquations.pdf</a></li>
<li> <a href='https://alamgirh.github.io/tutorial/latex-presentation-tutorial/ref.bib'>ref.bib</a></li>
<li> <a href='https://alamgirh.github.io/tutorial/latex-presentation-tutorial/QuadraticEquations.bbl'>QuadraticEquations.bbl</a></li>
<li> <a href='https://alamgirh.github.io/tutorial/latex-presentation-tutorial/quadraticplots.png'>quadraticplots.png</a></li>
</ul>
<p> ইতিমধ্যে আপনি গাণিতিক সমীকরণ, টেবিল তৈরি ও ছবি সংযুক্ত করা শিখে ফেলেছেন! এরপর ধীরে ধীরে আপনার মনে হাজারো প্রশ্ন তৈরি হবে। কিভাবে সমীকরণের নাম্বার লিখতে হয়, কিভাবে ডিফারেন্টিয়াল সমীকরণ লিখতে হয়, একাদিক ছবি থাকলে কিভাবে সংযুক্ত করতে হবে, কিভাবে টেবিলের সারি ও কলাম সংখ্যা বাড়াতে হবে কিংবা কমাতে হবে। এরকম হাজারো প্রশ্নের সমাধান দিয়ে দিবে google!</p>
