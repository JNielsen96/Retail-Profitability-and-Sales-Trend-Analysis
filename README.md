<h1> Data Carpentry: Cleaning and filtering receipts</h1>


<h2>Description</h2>
A Python script that parses unstructured, plain-text point-of-sale receipts and converts them into a structured JSON-style dictionary. The parser uses dynamically-built regex patterns to extract business details, cashier/customer info, itemised products (with quantity and per-unit price reconstruction), promotions/discounts, split payment methods, and transaction metadata (terminal, reference, GST, total). It's built as a single-pass, line-by-line state machine that tracks context (e.g. whether it's currently inside the "Payments" block, or buffering a product line waiting for its price) to correctly reconstruct multi-line records, then re-orders the output keys to match a required schema. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Python</b> 
- <b>json</b>
- <b>io / textwrap / itertools (test harness utilities)</b>


<h2>Environments Used </h2>

- <b>Windows 11</b>

<h2>Walk-through:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
