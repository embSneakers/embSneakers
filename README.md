# The Sneakers Project

This is the repository for the paper _"Using Web Data to Reveal 22-Year History of Sneaker Designs"_ submittted to **The Web Conference (WWW) 2022**.

### Data Description [(Data Link)](https://drive.google.com/drive/folders/1dYP4AFXGo_35-OS2yeRHeI4ZD_uFcPW_?usp=sharing)

#### 1. Overview
```
- We have crawled sneaker images and metadata from _StockX,_ a leading online resale shop at global scale.
- Total number of sneaker products crawled: 23,492 (see Table 1 for basic statistics)
- Due to the copyright issue, we cannot provide the original sneaker images.
- We share the data for our embedding results, SOTA embedding, and various engineered feature along with the crawled metadata
- See Section 2 for the details of each dataset.
```

<img src="./source/sneaker_table.jpg">
Table 1. Basic statistics of the crawled data.

#### 2. Dataset Description
```
df_512_mask_shape_210927.csv:
- Constructed embedding for the latent shape-invariant representation (top module in Figure 1)
- i.e., Color embedding

df_512_mask_color_210927.csv:
- Constructed embedding for the latent color-invariant representation (middle module in Figure 1)
- i.e., Shape embedding

df_512_mask_all_210927.csv:
- Constructed embedding for the latent all-invariant representation (top module in Figure 1)
- i.e., Combined embedding

df_384_looc.csv:
- Constructed embedding for the Leave-one-out Contrastive Learning (LooC)
- We consider this one as SOTA and compare our model with this one (Xiao et al, ICLR 2021)

total_df_RGBHSV_ent_seg_rgbHistBin128_meta.pkl:
- 
- 
```

<img src="./source/sneaker_embedding.jpg">
Figure 1. Illustration of the design embedding model.

#### 3. Code Description
```


```

#### 4. Additional Result

Below, we attach additional clustering results for the _combined embedding_, which were excluded from the manuscript due to page limit.

<img src="./source/combined_emb.jpg" style="width: 500px; height:auto;">
(a) K-means clustering result of the sneaker embedding for the combined attribute.
<br/><br/>

<img src="./source/combined_samples.jpg" style="width: 500px; height:auto;">
(b) Examples of sneaker products by cluster for the combined attribute.
Figure 2. Centroids within clusters and their 15-nearest neighbors based on the combined embedding.


<img src="./source/trend_sdi.jpg">



<br/>
We will disclose our contact information once the review period of WWW 2022 is ended.

<End of Document>


<!--
### Hi there 👋

**embSneakers/embSneakers** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
