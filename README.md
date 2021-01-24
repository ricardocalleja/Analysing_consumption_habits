<p><h1>Analysing consumption habits</h1></p>

During the pandemic caused by Sars-cov 19 I was in Chile as an inmigrant. I had just arrived on January 17th 2020 at the Capital Santiago with my mother, an eldery (74). Furtunately I found a convenient located appartment next to the supermarket "Lider" which is the Chilean version of Walmart.

Since the confinement started on March 22th. We decided to go out only once a week to buy groceries, preferably during non-busy hours (around 9am). Since I was unemployed I rigorously controled my budget, and doing so I kept all the receipts from the grocery store, then after almost a year I had 71 receipts from January 17th to September 28th of this peculiar 2020.

In the next lines I will show you How did I analyse the data from the groceries store's receipts.

<p><h1>The data</h1></p>
This is how one of those <a href="https://drive.google.com/file/d/1UBuSZwed86JgsYzJH0pmkTx4Lo_oitp1/view?usp=sharing">receipts</a> looks like. Well, my first approach to extract the data from the receipts was to scan it using th Goggle Drive functionality, and after that, to use google vision API to convert the pdf file to text and this was the <a href="https://drive.google.com/file/d/10v3jhFpseSjfe4ou2N1j2Wkr5FRd2wmK/view?usp=sharing" >result</a>. I asked for help on regular expressions and my friend @madacol helped me with this <a href="https://regex101.com/r/cr2Acv/3/">regex</a> that was able to detect 4 important fields (product_id, quantity, product_description and unit_price). But due to the format it only detected 26 out of 30 items in the receipt.

In order to find a solution to this issue I found that this particular company offered the option to download the receipt in a digital format through their website. So this was actually what I did. Since the original data was in a pdf format and not a scan like my previous try I found out that this helped a lot in data quality. Here is the same receipt but in it original pdf format.

Convinced that this was the best type for my data I manually downloaded the receipts. If anybody knows how to do it automatically please let me know. So, here you will find the <a href="https://drive.google.com/file/d/1cl0NC4IE9-H6zNncszAjTW1GglVdRhB-/view?usp=sharing">71 receipts</a>. I copy and pasted the context of the pdf files and using a regexp extracted the previously mentioned fields and put them in into excel to finally get this <a href= "https://drive.google.com/file/d/1dGW79fTzNIZ7-MvF3nmnR1hOYn71fTHU/view?usp=sharing">dataset</a>.
