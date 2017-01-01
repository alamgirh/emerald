---
layout: post
title: $\LaTeX$ ব্যবহার করে প্রেজেন্টেশন তৈরি (পর্ব ২) 
date: 2016-12-31
categories: update
author: Alamgir Hossain
tags: LaTeX Beamer Beginner
---

<img src="http://i.stack.imgur.com/zHFFO.png" class="fit image"> 

<h2> কিভাবে প্রেজেন্টেশন স্লাইডস গুলোকে আরো সুন্দর ভাবে তৈরি করবেন?</h2>

<p> অনেক ক্ষেত্রে দেখা যায় যিনি প্রেজেন্টেশন করছেন তিনি হয়তো সুন্দর ভাবে প্রেজেন্টেশন করতে পারছেন না। সেক্ষেত্রে যদি আপনার স্লাইডস গুলো এমন ভাবে তৈরী করেন যেন আপনার পাশাপাশি আপনার স্লাইডস গুলো কথা বলবে। এখানে আমি Overlays, Block ও Minipage এর কয়েকটি উদাহরণ দিলাম। এগুলো ব্যবহার করে আপনার স্লাইড গুলোকে আরো চমৎকার ভাবে তৈরী করতে পারেন। </p>

<h3> Overlays</h3>

<h4> Overlays - using pause </h4>

```LaTeX
\begin{frame}
  \frametitle{Overlays - using pause}

 \begin{itemize}
  \item
    $d \ge 0$; roots are real
    \pause 
    \begin{itemize}
  \item
    $d > 0$; roots are real and distinct
  \item
    $d = 0$; roots are real and same
    \end{itemize}
    \pause
  \item
    $d<0$; roots are complex
\end{itemize}

\end{frame}
```

<h4> Overlays - using item options </h4>

```LaTeX
\begin{frame}
  \frametitle{Overlays - using item options}

\begin{itemize}
    \item<1->   $d > 0$; roots are real and distinct
    \item<2->   $d = 0$; roots are real and same
    \item<3->   $d<0$; roots are complex
\end{itemize}

\end{frame}
```

<h4> Overlays - using different color </h4>

```LaTeX
\begin{frame}
  \frametitle{Overlays - using different color}

\begin{itemize}
    \item<1->   \alt<2>{\color{blue} $d > 0$; roots are real and distinct}{\color{gray} $d > 0$; roots are real and distinct}
    \item<1->   \alt<3>{\color{blue} $d = 0$; roots are real and same}{\color{gray} $d = 0$; roots are real and same}
    \item<1->  \alt<4>{\color{blue}  $d<0$; roots are complex}{\color{gray}$d<0$; roots are complex}
\end{itemize}

\end{frame}
```
<h4> Overlays - Table </h4>

```LaTeX
\begin{frame}
  \frametitle{Table: Overlay}
  \begin{center}
    \begin{tabular}{ll}
      \hline
      $d = b^2-4ac$ & comment about roots\\
      \hline \hline
      \onslide<2-> $d>0$ & roots are real and distinct\\
      \hline
      \onslide<3-> $d = 0$ & roots are real and same\\
      \hline
      \onslide<4-> $d<0$ & roots are complex\\
      \hline
    \end{tabular}
  \end{center}
\end{frame}
```

<h3> Block</h3>

```LaTeX
\begin{frame}
  \frametitle{Type of Roots}

  \begin{block}{Discriminant}
    $$d = b^2-4ac$$
    \end{block}
    
    \pause
    
    \begin{definition}
    Discriminant is 
    $$d = b^2-4ac$$
    \end{definition}
    
    \begin{exampleblock}{Matlab Code}
      $ d = b^2-4*a*c $   
    \end{exampleblock}

\end{frame}
```
<h3> Minipage</h3>

```LaTeX
\begin{frame}
  \frametitle{Minipage}
  \begin{minipage}{.5\textwidth}
    \begin{itemize}
        \item $d > 0$; roots are real and distinct
        \item $d = 0$; roots are real and same
        \item $d<0$; roots are complex
    \end{itemize}
    \end{minipage}
    ~
    \begin{minipage}{.4\textwidth}
    \begin{figure}
    \centering
    \includegraphics[scale=0.35]{quadraticplots.png}
    \caption{Quadratic Functions}
    \end{figure}
    \end{minipage}
\end{frame}
```
