# video_summarization
Summarizing medium-sized videos with a collection of images

At this stage uploaded notebooks check whether it is possible to cluster frames using their embeddings from some CNN model

Specifically, video_summarization_with_dl_embeddings_(part_I).ipynb is mostly a proof of concept and checks that: 
1) I can download videos from YouTube and process them using OpenCV
2) I can load pretrained GoogLeNet model and generate frame embeddings with it
3) I can meaningfully cluster video frames by checking t-sne projection of frame embeddings
