# video_summarization
Summarizing medium-sized videos with a collection of images

At this stage uploaded notebooks check whether it is possible to cluster frames using their embeddings from some CNN model

Specifically, video_summarization_with_dl_embeddings_(part_I).ipynb is mostly a proof of concept and checks that: 
1) I can download videos from YouTube and process them using OpenCV
2) I can load pretrained GoogLeNet model and generate frame embeddings with it
3) I can meaningfully cluster video frames by checking t-sne projection of frame embeddings

video_summarization_with_dl_embeddings_(part_II).ipynb actually tries to cluster video frames:
1) I applied GMM and K-Means (with euclidean and cosine distances) algorithms to cluster original and T-SNE projected video frame embeddigns
2) Found that applying clustering on T-SNE projections makes final results works
3) Found that simple K-Means can perform surprisingly well

In the next steps I will try to use mean-shift and DBSCAN algorithms to completely automate the process
