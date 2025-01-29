# Crypto Analysis Project

## Team Member
**Name:** Shravya Vorugallu  

## Classical Cipher Analyzed
**Cipher Type:** Monoalphabetic Substitution Cipher  


---

## Project Overview
This project focuses on the cryptanalysis of a **monoalphabetic substitution cipher**, a classical encryption technique where each letter in the plaintext is replaced with a fixed substitute. The primary objective is to recover the original plaintext without prior knowledge of the substitution key by leveraging statistical and computational techniques.

## Cryptanalysis Approach
Our method integrates **frequency analysis, bigram analysis, and Levenshtein distance calculations** to iteratively refine character mappings and identify the most probable plaintext match.

### Steps in the Cryptanalysis Process
1. **Character Frequency Analysis** – Identifies frequently occurring letters in the ciphertext and compares them to standard English letter frequencies.
2. **Segmenting the Text** – Breaks the ciphertext into smaller parts for better pattern recognition.
3. **Character Mapping Estimation** – Matches ciphertext characters to probable plaintext characters based on frequency distributions.
4. **Levenshtein Distance Calculation** – Measures similarity between the mapped ciphertext and candidate plaintexts.
5. **Bigram Analysis** – Considers common two-letter sequences to improve mapping accuracy.
6. **Scoring and Iteration** – Assigns scores based on similarity metrics and refines mappings over multiple iterations.
7. **Finding the Best Plaintext Match** – Determines the most likely original text based on cumulative scores.

## Extra Credit Analysis
- **Impact of Random Noise:** Assesses how increasing randomness in the ciphertext affects decryption success and runtime performance.
- **Effect of Candidate Plaintext Set Size:** Analyzes how adding more candidate plaintexts influences the cryptanalysis process.

## Results & Observations
- The approach is effective for structured monoalphabetic substitution ciphers.
- Performance decreases as randomness increases or as the candidate plaintext set grows significantly.
- The method is computationally intensive but successfully recovers plaintexts when statistical patterns are preserved.

## Conclusion
This project demonstrates a systematic approach to breaking monoalphabetic substitution ciphers using statistical and computational techniques. The iterative refinement process and incorporation of multiple linguistic patterns enhance the accuracy of plaintext recovery.

---

## Usage Instructions
### Requirements
- Python 3.x
- Required Libraries: `numpy`, `nltk`, `Levenshtein`

### Running the Code
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the cryptanalysis script:
   ```bash
   python decrypt.py <ciphertext_file>
   ```

### Example
```bash
python decrypt.py ciphertext.txt
```

## Contact
For any questions, please contact **Shravya Vorugallu**.

