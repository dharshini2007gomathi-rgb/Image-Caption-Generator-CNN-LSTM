📝 Text Preprocessing

The captions are processed before being given to the LSTM model.

The preprocessing steps include:

Converting text into lowercase
Removing unnecessary punctuation
Tokenization
Vocabulary creation
Converting words into numerical sequences
Adding start and end tokens
Padding the sequences
🔧 Model Training

The CNN-LSTM model is trained using the preprocessed Flickr8K images and captions.

During training:

Image features are extracted using CNN.
Captions are tokenized and converted into numerical sequences.
Image features and caption sequences are provided to the model.
The LSTM predicts the next word.
The predicted word is compared with the actual word.
The model parameters are updated based on the prediction error.
The training process is repeated for multiple epochs.
✨ Caption Generation

After training, a new image is provided as input to the system.

The CNN extracts visual features from the image. The LSTM then generates the caption one word at a time.

The process starts with a start token and continues until the end token is generated or the maximum sequence length is reached.

🔍 Caption Generation Methods

The project uses two caption generation approaches:

Greedy Search

Greedy Search selects the word with the highest probability at each prediction step.

Beam Search

Beam Search considers multiple possible word sequences and selects a suitable overall caption sequence.

These approaches help compare different caption generation results.

📈 Model Evaluation

The generated captions are compared with the actual captions available in the dataset.

The project uses BLEU score to evaluate the similarity between generated captions and reference captions.

The evaluation compares:

Actual captions
Greedy Search generated captions
Beam Search generated captions
BLEU score
📊 Visualization

The project provides visualization of randomly selected test images along with their actual and generated captions.

The visualization helps to understand how effectively the model generates captions based on the visual content of the images.

📁 Project Structure
Image-Caption-Generator-CNN-LSTM/
│
├── README.md
└── image-caption123.ipynb
🛠️ Technologies Used
Python
TensorFlow
Keras
NumPy
Pandas
Matplotlib
Natural Language Processing
CNN
LSTM
Google Colab
Jupyter Notebook
▶️ Running the Project

The project notebook can be opened using:

Google Colab
Jupyter Notebook
JupyterLab
VS Code with Jupyter extension

Run the notebook cells sequentially to perform preprocessing, image feature extraction, model training, caption generation, and evaluation.

🎯 Learning Objectives

Through this project, the following concepts were explored:

Image preprocessing
CNN architecture
Image feature extraction
Text preprocessing
Tokenization
Word embedding
LSTM sequence learning
Next-word prediction
Image caption generation
Greedy Search
Beam Search
BLEU score evaluation
Deep Learning
📌 Key Outcome

The developed CNN-LSTM model is able to generate textual descriptions for input images by combining visual features extracted using CNN with sequential language learning using LSTM.

The generated captions demonstrate the ability of the model to connect image content with natural language descriptions.

👩‍💻 Author

Dharshini

B.Tech Artificial Intelligence and Data Science

🙏 Acknowledgements
Flickr8K Dataset
TensorFlow / Keras
Google Colab
Deep Learning and Natural Language Processing resources
