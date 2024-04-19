
## Prerequisites -

- Python 3.10.6 (while creating new envirronment put this version as it is needed for torch dependencies)


### 3. Install Python 3.10.6

Download and install [Python 3.10.6](https://www.python.org/downloads/release/python-3106) if not installed already.
(I recommend using this version for compatibility with the torch dependencies)

### 4. Clone Main Repository

Clone the main repository & move into the directory:

```bash
git clone https://github.com/sockthem/gg
cd AI-Generated-Text-Detection
```

### 5. Download Weights

Download the model [Weights](https://www.mediafire.com/file/7n4b2e1geeuzu69/weights.zip/file) (~9GB) from [here](https://www.mediafire.com/file/7n4b2e1geeuzu69/weights.zip/file) & extract them to the weights directory:

```bash
# wget https://www.mediafire.com/file/7n4b2e1geeuzu69/weights.zip/file -O weights.zip
unzip weights.zip -d ./weights
```

### 6. Create and Activate Virtual Environment

Create and activate the virtual environment:

```bash
python -m venv env
source env/bin/activate
```

### 8. Install Requirements

Install project requirements:

```bash
pip install -r packages.txt
```

### 9. Run the Application

Run the app.py file,
(make sure to adjust the params in the config.py file):

```bash
python app.py
```

### 10. Clone Frontend Repository

clone the frontend repository & move into the directory:

```bash
cd ../
git clone https://github.com/jesvijonathan/Snitch-GPT-Frontend
cd Snitch-GPT-Frontend
```

### 11. Install NPM Dependencies and Build App

Install npm project dependencies and build the app:

```bash
npm install
npm run build
```

### 12. Run Frontend Application

Run the frontend application:

```bash
npm run dev
```

### 13. Open Application

Open the application in your web browser:

```bash
http://localhost:5173 # for App
http://localhost:5000 # for API
```

## Notes

- Use the application via API or web interface.
- Refer to the [frontend repository](https://github.com/jesvijonathan/Snitch-GPT-Frontend) for more details.
- Both the frontend and backend applications should be running simultaneously.
- Configure the parameters in the `config.py` file for better results.
- Ensure you have the recommended hardware and software requirements:
  - **GPU Mode** (recommended, significantly better performance),
    - CUDA enabled GPU,
    - 4GB+ VRAM (with all 6 models loaded, 12GB+ recommended),
  - **CPU Mode** (not recommended, although you can use it in MIX mode alongside GPU),
    - 4+ Core CPU (8+ Core CPU recommended),
    - 2.5GHz+ Clock Speed,
    - 16GB RAM (32GB+ recommended)
  - Min 40GB Storage (SSD recommended, faster swap & loading time),
  - Python 3.10.6
- Lack of memory or VRAM may cause poor performance or might crash during execution.
- Lack of storage may cause the program to crash due insufficient space for model weights or swap memory.
- Switch to sequential mode & disable models to reduce memory usage if you face memory issues.
  <br>
- This project works best with text with more than 250 characters & is trained on lengthy texts & using bert/DebertaModel along with 3M GPT-4 Data.
- Use this project along with the frontend interface intended to use with this project, which has visualization & more | [Snitch-GPT](https://snitch-gpt.vercel.app)
- Adjust the params in the config.py file best, as per need
- The model is trained on a large custom dataset for the most accurate results. Results may not always be inaccurate, use at own risk.
- I know most of it is speghetti code rn, but it works. Will refactor soon. 0_0

## Features

- Detect AI-generated text/content.
- Score the content based on multiple parameters & the probability of being AI-generated.
- Model trained on a broader/large dataset for the most accurate results.
- Use of new multiple models & techniques to improve the accuracy of the model.
- Interactive Web app interface to interact with the application.
- API availability to integrate the application with other services.
- Minimal & easy to use, can save research time.
- Customizable parameters to adjust the model for better results.
- Maximum efficiency by using max hardware resources for significant performance boosts & faster results.
- Supports one shot detection & other checks.
- ~300ms execution time for optimal cases.
- many more...