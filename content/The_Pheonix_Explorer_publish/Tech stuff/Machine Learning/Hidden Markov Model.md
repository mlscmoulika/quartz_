To get a context of HMM, please also refer to [[Markov Model]] before.

HMM consists of Hidden states and observed states. In a short summary, looking at the observed states, we try to determine the hidden state. The key is to determine the probability to transition from one state to another. And then based on the Markovian assumption that, any state depends on the previous state, one can simplify the probability expression, and make computations.

### Category of problem statements that could be solved using this model are as follows:
1. **Sequence Likelihood Prediction**:
    
    - **Task**: Compute the probability of observing a sequence given the HMM.
    - **Example**: How likely is a given DNA sequence in a biological context?
2. **Sequence Classification**:
    
    - **Task**: Determine the most likely category for a given sequence.
    - **Example**: Classify a time series as "walking" or "running."
3. **Prediction of the Next Step**:
    
    - **Task**: Predict future observations or hidden states based on past data.
    - **Example**: Predict the next word in a sentence.

### Some popular problem statements :
1. **Speech Recognition**:
    
    - Hidden states: Phonemes or speech sounds.
    - Observed states: Audio features like MFCCs (Mel-frequency cepstral coefficients).
2. **Part-of-Speech Tagging**:
    
    - Hidden states: Parts of speech (e.g., noun, verb).
    - Observed states: Words in a sentence.
3. **Gene Sequencing**:
    
    - Hidden states: Gene functions or regulatory regions.
    - Observed states: Nucleotide sequences (A, C, G, T).

### How to model it?
- 1. **Define Initial Parameters**:
    - **State Space**: The set of possible hidden states.
    - **Transition Probabilities**: Initial probabilities for transitioning between states.
    - **Emission Probabilities**: Initial probabilities for emitting observed states from hidden states.
2. **Train the Model**:
    - Use **Baum-Welch Algorithm** or similar Expectation-Maximization approaches.
    - Input: Training data with observed sequences and, optionally, labeled hidden states.
    - Output: Refined transition and emission probabilities.
3. **Test the Model**:
    - Use separate test data to validate.
    - Compute metrics like **sequence likelihood**, **classification accuracy**, or **prediction accuracy** depending on the task.


#Machine-learning
