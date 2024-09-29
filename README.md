
<div id="header" align="center" class="markdown prose w-full break-words dark:prose-invert dark"><p>Howdy! 👋<br> I'm Deny. <br></p>
  <img src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" width="100"/>
<div id="badges">
  <a href="https://www.linkedin.com/in/deny-tran-dfw/">
    <img src="https://github.com/TranDenyDFW/TranDenyDFW/blob/main/assets/li.png" alt="LinkedInBadge"  style="border: 15px solid transparent; width: 100px; height: 40px;" /> 
  </a>&nbsp;&nbsp;
  <a href="https://learn.microsoft.com/en-us/users/denytrandfw/">
    <img src="https://github.com/TranDenyDFW/TranDenyDFW/blob/main/assets/ms.png" alt="MicrosoftLearningBadge"  style="border: 15px solid transparent; width: 100px; height: 40px;" /> 
  </a>&nbsp;&nbsp;
  <a href="https://huggingface.co/DenyTranDFW">
    <img src="https://github.com/TranDenyDFW/TranDenyDFW/blob/main/assets/hf.png" alt="HuggingFaceBadge"  style="border: 15px solid transparent; width: 100px; height: 40px;" /> 
  </a>&nbsp;&nbsp;
  <a href="https://www.kaggle.com/denytran">
    <img src="https://github.com/TranDenyDFW/TranDenyDFW/blob/main/assets/kg.png" alt="KaggleBadge"  style="border: 15px solid transparent; width: 100px; height: 40px;" /> 
  </a>
</div>
<hr>
<div align="left">
<h2>About Me</h2>
<p>I've spent my entire professional career in Information Technology, moving through roles from Help Desk to Network Cable Installation and Inventory Manager. Lately, I’ve realized that in my last few jobs, I tended to follow a familiar pattern: I’d jump in, learn the ropes quickly, and then find myself spending my free time creating solutions on "How to make my job easier."</p><p>What started with Excel and VBA has evolved into a deeper dive into Python and SQL. This is me taking a big step in a different direction, embracing my passion for coding and analysis!</p></div>
<div align="left">  <br>
<h2>Self-Concocted SQL-/ETL-/ML-Related Stuff</h2>
<h4><i> <a href="https://huggingface.co/datasets/DenyTranDFW/SEC-Financial-Statements-And-Notes-Dataset">SEC-Financial-Statements-And-Notes-Dataset</a></i></h4>

- Built from the [SEC's Financial Statements & Notes](https://www.sec.gov/data-research/financial-statement-notes-data-sets) .tsv datasets.
- Environment: Docker on Ubuntu w/SQL Server 2019.
- Joins/keys were based on guidance from [FSNDS Notes](https://www.sec.gov/files/aqfsn_1.pdf), but the results were mainly trial and error due to the quality of the dataset.  
- Configurations were based on general SQL best practices, including bit and pieces of ideas from the following fantastic works:
  - [Expert Performance Indexing in Azure SQL and SQL Server 2022, Edward Pollack, Jason Strate](https://www.amazon.com/Expert-Performance-Indexing-Azure-Server/dp/1484292146)
  - [Effective SQL - 61 Specific Ways to Write Better SQL, John L. Viescas, Douglas J. Steele, Ben G. Clothier](https://www.amazon.com/Effective-SQL-Specific-Software-Development/dp/0134578899)
  - [SQL Antipatterns, Bill Karwin](https://www.amazon.com/SQL-Antipatterns-Programming-Pragmatic-Programmers/dp/1934356557)
  - [SQL Queries for Mere Mortals, John Viescas](https://www.amazon.com/SQL-Queries-Mere-Mortals-Hands/dp/0134858336)
- The toughest part was trying to deal with such a large amount of data when never having done something like this before. After shedding many tears and breaking many more databases, it was smooth sailing.

<br>
<h4><i> <a href="https://www.kaggle.com/code/denytran/10-year-auto-loans-a-z-starter-pyspark-duckdb">Analysis of 10-Year Auto-Loan Payments</a></i></h4>

- Based on one of the many parsed [SEC's ABS-EE (Asset Backed Securities - Electronic Exhibits)](https://huggingface.co/DenyTranDFW) XML datasets.
- Purpose of illustration was more-or-less for:
  - Testing the parsed datasets,
  - practicing SQL,
  - working with ML models/libraries, and
  - working with PySpark
- Some key takeaways here were:
  - PySpark is very good with working with large amounts of data, but is a different story when trying to get it to use the GPU.
    - It's nice that PySpark developers have ML options, but for serious work, you'll likely have to use PyTorch or TensorFlow.
  - DuckDB is amazing. It handled the 35M+ rows here easily. On top of that (prior to this), the 550M+ rows of data from the FSNDS was easily consumed and queried.
    - With that said, DuckDB will only work well if you let it do the indexing. For example, if you tried to add all the FSNDS primary/foreign keys, it'll become unresponsive during data insert.
    - So, a good quick go-to for big datasets. But not so much if you're looking for something more.
<br>
<h4><i> <a href="https://www.kaggle.com/code/denytran/hugging-face-fsnonotesdatasets-starter">Financial Statements And No-Notes Datasets</a></i></h4>

- This was an extraction of the [FSNDS](https://huggingface.co/datasets/DenyTranDFW/SEC-Financial-Statements-And-Notes-Dataset) to test the quality of the data after it was exported from SQL Server.

<br>
<h4><i> <a href="https://www.kaggle.com/code/denytran/tabular-financial-data-generator">Tabular Data Generator</a></i></h4>

- Similarly, an extraction of the [FSNDS](https://huggingface.co/datasets/DenyTranDFW/SEC-Financial-Statements-And-Notes-Dataset), but used here instead, for creating training data for a Tabular LLM (i.e., [TaBERT](https://github.com/facebookresearch/TaBERT)).

<br>
<h4><i> <a href="https://huggingface.co/DenyTranDFW/gpt2-next-tag-prediction">GPT2 - Predicting Financial Statement Line Items</a></i></h4>

- Here, we train a GPT2 model on XBRL tags (i.e., AssetsCurrent) for next-word prediction (statement line item).
- This was based primarily on curiosity, since we know that if we tell a model something enough times, it'll remember it.
- The results though, was somewhat enlightening:
  - When given: "AssetsCurrent", rather than returning the tag (i.e., "PropertyPlantAndEquipmentNet"), the model would return "Property"
  - This is likely because it was initially trained to know that "PropertyPlantAndEquipmentNet" are composed of multiple words, so, 10-epochs of 35000 XBRL tags will likely not change the fact that "Property" is the valid next word.



