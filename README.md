
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
<h2>Self-Concocted SQL-/ETL-/ML-/Analyst-Related Stuff</h2>
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

<center>
<img src="[https://cdn-lfs-us-1.hf.co/repos/d9/68/d968a759e896eb8a5136c6a26499f087fe3a8108c8cd8547e727a72c1c346d84/1266fd9924f81703a62dd1e4878c814c17542086b9a3d6e178cfff3094d383a7?response-content-disposition=inline%3B+filename*%3DUTF-8%27%27fsnds-graph.png%3B+filename%3D%22fsnds-graph.png%22%3B&response-content-type=image%2Fpng&Expires=1727996552&Policy=eyJTdGF0ZW1lbnQiOlt7IkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTcyNzk5NjU1Mn19LCJSZXNvdXJjZSI6Imh0dHBzOi8vY2RuLWxmcy11cy0xLmhmLmNvL3JlcG9zL2Q5LzY4L2Q5NjhhNzU5ZTg5NmViOGE1MTM2YzZhMjY0OTlmMDg3ZmUzYTgxMDhjOGNkODU0N2U3MjdhNzJjMWMzNDZkODQvMTI2NmZkOTkyNGY4MTcwM2E2MmRkMWU0ODc4YzgxNGMxNzU0MjA4NmI5YTNkNmUxNzhjZmZmMzA5NGQzODNhNz9yZXNwb25zZS1jb250ZW50LWRpc3Bvc2l0aW9uPSomcmVzcG9uc2UtY29udGVudC10eXBlPSoifV19&Signature=kNyzXarMZmGYpf3%7ENhV97JLn83ZcEqpTuIZRPOr28Hs21omTgIxaCZIaxVDU3JYl-ZdbITaXpwpPRLoDZcQikZ4jzd%7EAjyd5CpoYF--oIDm0eZIYlXvNqY6%7ESdrdEP0LnaO4lgRX0lXrW0qeV6nWkCONkqHT3a6CF6EV-suckxU5kfvar6481MlUj4yQY3dC0EM4ut7r0IN3T6SLbUCy2MRyj3DJEz-i-DLjfY5NEX32yu4XNDBCF2Fnj8Ga-H%7EbMm5elNDTpgQjL4giwWIVWO-xvW4pncCNj%7EYd7BJqFcKynpUZ9OTGsxVPlaIsJ7y10DP1TCj44waGuazo8EVEiA__&Key-Pair-Id=K24J24Z295AEI9](https://media.licdn.com/dms/image/v2/D562DAQHHmPkwMbiv6Q/profile-treasury-image-shrink_1280_1280/profile-treasury-image-shrink_1280_1280/0/1728121554171?e=1728752400&v=beta&t=2thwlGHuRiV2lRrrO38pyMr9JBSdL2wBeLz59i_v8dQ)" alt="fsnds_graph" width="800" height="800"></center>

<br>
<h4><i> <a href="https://www.kaggle.com/code/denytran/10-year-auto-loans-a-z-starter-pyspark-duckdb">10-Year Auto-Loan Payments + PySpark ML</a></i></h4>

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
<h4><i> <a href="https://github.com/TranDenyDFW/Excel_Operating_Model">Excel Operating Model</a></i></h4>

- A financial model I created back in 2017 from scraped data.
- The way the data is stored is somewhat naive, but the project as a whole was nonetheless, enlightening.

![operating_model](https://github.com/TranDenyDFW/Excel_Operating_Model/blob/main/operating_model.png)


