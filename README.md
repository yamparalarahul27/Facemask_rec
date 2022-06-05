Hi People This is Yamparala Rahul
I am greatful to see you here, this projec is my college final year project done in 2022 June. 
I don't clame full originality of the code, as this is some modified one found from different sources. 
Thnakyou and Have a great day.

Running the code - 
1. Donwnload/Clone repository.
2. Add images with mask and without mask in the dataset folder under respective name.
3. Create embedding for the face using command
'python extract_embeddings.py --dataset dataset  --embeddings output/embeddings.pickle  --detector face_detection_model  --embedding-model openface_nn4.small2.v1.t7'
4. Train the model so it recognizes each face at real time. Command:
'python train_model.py --embeddings output/embeddings.pickle --recognizer output/recognizer.pickle --le output/le.pickle'
5. Test the model if it recognizes faces correctly. Command:
'python recognize_video.py --detector face_detection_model --embedding-model openface_nn4.small2.v1.t7 --recognizer output/recognizer.pickle --le output/le.pickle'
