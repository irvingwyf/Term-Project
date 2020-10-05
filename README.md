# Term-Project
multi-speaker identification 
#Literature Review:
Speaker Diarization:
•	Speech Detection: Extract speech part in one audio recording using a Voice Activity Detector (VAD) module.
•	Speech Segmentation: Extract out small segments of your audio call in a continuous manner.
•	Embedding Extraction: This system creates a neural-network based embedding of your speech segments extracted in the previous step. An embedding is a vector representation of data which could be used by the deep learning framework.
•	Clustering: Cluster embeddings we created above and the system will training itself by using supervised learning method in order to identify which embeddings are belong to same speaker and assigned the label of that speaker as well.
•	Transcription: Segment out the audio into clips belonging to each speaker, and pass it to a Speech-to-Text model (or ASR) which produces the transcript of the speech segment.
