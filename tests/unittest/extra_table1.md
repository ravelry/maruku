Write a comment abouth the test here.
*** Markdown input: ***
CSS: style.css

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

***

| Item      | Value |
| --------- | -----:|
| Computer  | $1600 |
| Phone     |   $12 |
| Pipe      |    $1 |

***

| Function name | Description                    |
| ------------- | ------------------------------ |
| `help()`      | Display the help window.       |
| `destroy()`   | **Destroy your computer!**     |


***

| Very long long head  | 
| :------------        | 
| left                 | 

***

| Very long long head  | 
| -------------------: | 
| right                |

***

| Very long long head  | 
| :------------------: | 
| center               |
*** Output of to_html ***
<table
      ><thead
        ><tr
          ><th>First Header</th
          ><th>Second Header</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: left;'>Content Cell</td
          ><td style='text-align: left;'>Content Cell</td
        ></tr
        ><tr
          ><td style='text-align: left;'>Content Cell</td
          ><td style='text-align: left;'>Content Cell</td
        ></tr
      ></tbody
    ></table
    ><hr
    /><table
      ><thead
        ><tr
          ><th>Item</th
          ><th>Value</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: left;'>Computer</td
          ><td style='text-align: right;'>$1600</td
        ></tr
        ><tr
          ><td style='text-align: left;'>Phone</td
          ><td style='text-align: right;'>$12</td
        ></tr
        ><tr
          ><td style='text-align: left;'>Pipe</td
          ><td style='text-align: right;'>$1</td
        ></tr
      ></tbody
    ></table
    ><hr
    /><table
      ><thead
        ><tr
          ><th>Function name</th
          ><th>Description</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: left;'
            ><tt>help()</tt
          ></td
          ><td style='text-align: left;'>Display the help window.</td
        ></tr
        ><tr
          ><td style='text-align: left;'
            ><tt>destroy()</tt
          ></td
          ><td style='text-align: left;'
            ><strong>Destroy your computer!</strong
          ></td
        ></tr
      ></tbody
    ></table
    ><hr
    /><table
      ><thead
        ><tr
          ><th>Very long long head</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: left;'>left</td
        ></tr
      ></tbody
    ></table
    ><hr
    /><table
      ><thead
        ><tr
          ><th>Very long long head</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: right;'>right</td
        ></tr
      ></tbody
    ></table
    ><hr
    /><table
      ><thead
        ><tr
          ><th>Very long long head</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: center;'>center</td
        ></tr
      ></tbody
    ></table
  >
*** Output of to_latex ***
\begin{tabular}{l|l}
First Header&Second Header\\
\hline 
Content Cell&Content Cell\\
Content Cell&Content Cell\\
\end{tabular}


\vspace{.5em} \hrule \vspace{.5em}
\begin{tabular}{l|r}
Item&Value\\
\hline 
Computer&\$1600\\
Phone&\$12\\
Pipe&\$1\\
\end{tabular}


\vspace{.5em} \hrule \vspace{.5em}
\begin{tabular}{l|l}
Function name&Description\\
\hline 
\colorbox[rgb]{0.94,0.94,0.88}{\tt \char104\char101\char108\char112\char40\char41}&Display the help window.\\
\colorbox[rgb]{0.94,0.94,0.88}{\tt \char100\char101\char115\char116\char114\char111\char121\char40\char41}&{\bf Destroy your computer!}\\
\end{tabular}


\vspace{.5em} \hrule \vspace{.5em}
\begin{tabular}{l}
Very long long head\\
\hline 
left\\
\end{tabular}


\vspace{.5em} \hrule \vspace{.5em}
\begin{tabular}{r}
Very long long head\\
\hline 
right\\
\end{tabular}


\vspace{.5em} \hrule \vspace{.5em}
\begin{tabular}{c}
Very long long head\\
\hline 
center\\
\end{tabular}


*** Output of to_s ***
First HeaderSecond HeaderContent CellContent CellContent CellContent CellItemValueComputer$1600Phone$12Pipe$1Function nameDescriptionDisplay the help window.Destroy your computer!Very long long headleftVery long long headrightVery long long headcenter
*** Output of to_s ***
First HeaderSecond HeaderContent CellContent CellContent CellContent CellItemValueComputer$1600Phone$12Pipe$1Function nameDescriptionDisplay the help window.Destroy your computer!Very long long headleftVery long long headrightVery long long headcenter
*** Output of inspect ***
MDElement.new(:document,[	
	MDElement.new(:table,[	
		MDElement.new(:head_cell,[	
			"First Header"
		], {}),
		
		MDElement.new(:head_cell,[	
			"Second Header"
		], {}),
		
		MDElement.new(:cell,[	
			"Content Cell"
		], {}),
		
		MDElement.new(:cell,[	
			"Content Cell"
		], {}),
		
		MDElement.new(:cell,[	
			"Content Cell"
		], {}),
		
		MDElement.new(:cell,[	
			"Content Cell"
		], {})
	], {:align=>[:left, :left]}),
	
	MDElement.new(:hrule,[],{}),
	
	MDElement.new(:table,[	
		MDElement.new(:head_cell,[	
			"Item"
		], {}),
		
		MDElement.new(:head_cell,[	
			"Value"
		], {}),
		
		MDElement.new(:cell,[	
			"Computer"
		], {}),
		
		MDElement.new(:cell,[	
			"$1600"
		], {}),
		
		MDElement.new(:cell,[	
			"Phone"
		], {}),
		
		MDElement.new(:cell,[	
			"$12"
		], {}),
		
		MDElement.new(:cell,[	
			"Pipe"
		], {}),
		
		MDElement.new(:cell,[	
			"$1"
		], {})
	], {:align=>[:left, :right]}),
	
	MDElement.new(:hrule,[],{}),
	
	MDElement.new(:table,[	
		MDElement.new(:head_cell,[	
			"Function name"
		], {}),
		
		MDElement.new(:head_cell,[	
			"Description"
		], {}),
		
		MDElement.new(:cell,[	
			MDElement.new(:inline_code,[],{:raw_code=>"help()"})
		], {}),
		
		MDElement.new(:cell,[	
			"Display the help window."
		], {}),
		
		MDElement.new(:cell,[	
			MDElement.new(:inline_code,[],{:raw_code=>"destroy()"})
		], {}),
		
		MDElement.new(:cell,[	
			MDElement.new(:strong,[	
				"Destroy your computer!"
			], {})
		], {})
	], {:align=>[:left, :left]}),
	
	MDElement.new(:hrule,[],{}),
	
	MDElement.new(:table,[	
		MDElement.new(:head_cell,[	
			"Very long long head"
		], {}),
		
		MDElement.new(:cell,[	
			"left"
		], {})
	], {:align=>[:left]}),
	
	MDElement.new(:hrule,[],{}),
	
	MDElement.new(:table,[	
		MDElement.new(:head_cell,[	
			"Very long long head"
		], {}),
		
		MDElement.new(:cell,[	
			"right"
		], {})
	], {:align=>[:right]}),
	
	MDElement.new(:hrule,[],{}),
	
	MDElement.new(:table,[	
		MDElement.new(:head_cell,[	
			"Very long long head"
		], {}),
		
		MDElement.new(:cell,[	
			"center"
		], {})
	], {:align=>[:center]})
], {:css=>"style.css"})
*** EOF ***




Failed tests:   [:to_html, :inspect] 
And the following are the actual outputs for methods:
   [:to_html, :to_latex, :to_s, :to_s, :inspect]:


*** Output of to_html ***
-----| WARNING | -----
<table
      ><thead
        ><tr
          ><th>First Header</th
          ><th>Second Header</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: left;'>Content Cell</td
          ><td style='text-align: left;'>Content Cell</td
        ></tr
        ><tr
          ><td style='text-align: left;'>Content Cell</td
          ><td style='text-align: left;'>Content Cell</td
        ></tr
      ></tbody
    ></table
    ><hr
    /><table
      ><thead
        ><tr
          ><th>Item</th
          ><th>Value</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: left;'>Computer</td
          ><td style='text-align: right;'>$1600</td
        ></tr
        ><tr
          ><td style='text-align: left;'>Phone</td
          ><td style='text-align: right;'>$12</td
        ></tr
        ><tr
          ><td style='text-align: left;'>Pipe</td
          ><td style='text-align: right;'>$1</td
        ></tr
      ></tbody
    ></table
    ><hr
    /><table
      ><thead
        ><tr
          ><th>Function name</th
          ><th>Description</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: left;'
            ><code>help()</code
          ></td
          ><td style='text-align: left;'>Display the help window.</td
        ></tr
        ><tr
          ><td style='text-align: left;'
            ><code>destroy()</code
          ></td
          ><td style='text-align: left;'
            ><strong>Destroy your computer!</strong
          ></td
        ></tr
      ></tbody
    ></table
    ><hr
    /><table
      ><thead
        ><tr
          ><th>Very long long head</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: left;'>left</td
        ></tr
      ></tbody
    ></table
    ><hr
    /><table
      ><thead
        ><tr
          ><th>Very long long head</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: right;'>right</td
        ></tr
      ></tbody
    ></table
    ><hr
    /><table
      ><thead
        ><tr
          ><th>Very long long head</th
        ></tr
      ></thead
      ><tbody
        ><tr
          ><td style='text-align: center;'>center</td
        ></tr
      ></tbody
    ></table
  >
*** Output of to_latex ***
\begin{tabular}{l|l}
First Header&Second Header\\
\hline 
Content Cell&Content Cell\\
Content Cell&Content Cell\\
\end{tabular}


\vspace{.5em} \hrule \vspace{.5em}
\begin{tabular}{l|r}
Item&Value\\
\hline 
Computer&\$1600\\
Phone&\$12\\
Pipe&\$1\\
\end{tabular}


\vspace{.5em} \hrule \vspace{.5em}
\begin{tabular}{l|l}
Function name&Description\\
\hline 
\colorbox[rgb]{0.94,0.94,0.88}{\tt \char104\char101\char108\char112\char40\char41}&Display the help window.\\
\colorbox[rgb]{0.94,0.94,0.88}{\tt \char100\char101\char115\char116\char114\char111\char121\char40\char41}&{\bf Destroy your computer!}\\
\end{tabular}


\vspace{.5em} \hrule \vspace{.5em}
\begin{tabular}{l}
Very long long head\\
\hline 
left\\
\end{tabular}


\vspace{.5em} \hrule \vspace{.5em}
\begin{tabular}{r}
Very long long head\\
\hline 
right\\
\end{tabular}


\vspace{.5em} \hrule \vspace{.5em}
\begin{tabular}{c}
Very long long head\\
\hline 
center\\
\end{tabular}


*** Output of to_s ***
First HeaderSecond HeaderContent CellContent CellContent CellContent CellItemValueComputer$1600Phone$12Pipe$1Function nameDescriptionDisplay the help window.Destroy your computer!Very long long headleftVery long long headrightVery long long headcenter
*** Output of to_s ***
First HeaderSecond HeaderContent CellContent CellContent CellContent CellItemValueComputer$1600Phone$12Pipe$1Function nameDescriptionDisplay the help window.Destroy your computer!Very long long headleftVery long long headrightVery long long headcenter
*** Output of inspect ***
-----| WARNING | -----
md_el(:document,[
	md_el(:table,[
		md_el(:head_cell,[	"First Header"]),
		md_el(:head_cell,[	"Second Header"]),
		md_el(:cell,[	"Content Cell"]),
		md_el(:cell,[	"Content Cell"]),
		md_el(:cell,[	"Content Cell"]),
		md_el(:cell,[	"Content Cell"])
	], {:align=>[:left, :left]}),
	md_el(:hrule,[]),
	md_el(:table,[
		md_el(:head_cell,[	"Item"]),
		md_el(:head_cell,[	"Value"]),
		md_el(:cell,[	"Computer"]),
		md_el(:cell,[	"$1600"]),
		md_el(:cell,[	"Phone"]),
		md_el(:cell,[	"$12"]),
		md_el(:cell,[	"Pipe"]),
		md_el(:cell,[	"$1"])
	], {:align=>[:left, :right]}),
	md_el(:hrule,[]),
	md_el(:table,[
		md_el(:head_cell,[	"Function name"]),
		md_el(:head_cell,[	"Description"]),
		md_el(:cell,[	md_el(:inline_code,[], {:raw_code=>"help()"})]),
		md_el(:cell,[	"Display the help window."]),
		md_el(:cell,[	md_el(:inline_code,[], {:raw_code=>"destroy()"})]),
		md_el(:cell,[	md_el(:strong,[	"Destroy your computer!"])])
	], {:align=>[:left, :left]}),
	md_el(:hrule,[]),
	md_el(:table,[
		md_el(:head_cell,[	"Very long long head"]),
		md_el(:cell,[	"left"])
	], {:align=>[:left]}),
	md_el(:hrule,[]),
	md_el(:table,[
		md_el(:head_cell,[	"Very long long head"]),
		md_el(:cell,[	"right"])
	], {:align=>[:right]}),
	md_el(:hrule,[]),
	md_el(:table,[
		md_el(:head_cell,[	"Very long long head"]),
		md_el(:cell,[	"center"])
	], {:align=>[:center]})
], {:css=>"style.css"})
*** Output of Markdown.pl ***
<p>CSS: style.css</p>

<p>First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell</p>

<hr />

<p>| Item      | Value |
| --------- | -----:|
| Computer  | $1600 |
| Phone     |   $12 |
| Pipe      |    $1 |</p>

<hr />

<p>| Function name | Description                    |
| ------------- | ------------------------------ |
| <code>help()</code>      | Display the help window.       |
| <code>destroy()</code>   | <strong>Destroy your computer!</strong>     |</p>

<hr />

<p>| Very long long head  | 
| :------------        | 
| left                 | </p>

<hr />

<p>| Very long long head  | 
| -------------------: | 
| right                |</p>

<hr />

<p>| Very long long head  | 
| :------------------: | 
| center               |</p>

*** Output of Markdown.pl (parsed) ***
<p>CSS: style.css</p
    ><p>First Header | Second Header
------------- | -------------
Content Cell | Content Cell
Content Cell | Content Cell</p
    ><hr
    /><p>| Item | Value |
| --------- | -----:|
| Computer | $1600 |
| Phone | $12 |
| Pipe | $1 |</p
    ><hr
    /><p>| Function name | Description |
| ------------- | ------------------------------ |
| <code>help()</code
      > | Display the help window. |
| <code>destroy()</code
      > | <strong>Destroy your computer!</strong
      > |</p
    ><hr
    /><p>| Very long long head | 
| :------------ | 
| left | </p
    ><hr
    /><p>| Very long long head | 
| -------------------: | 
| right |</p
    ><hr
    /><p>| Very long long head | 
| :------------------: | 
| center |</p
  >