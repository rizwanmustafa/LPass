# Preview
![LPass Preview](./demonstration.gif)

# Requirements
- Python3 (For running the code)
- Mariadb / MySQL (For storing the credentials)

# Build instructions

1. Create a new virtual environment in a folder called 'venv' for this project (This will prevent your binary size and compilation time from being too long).
```bash
python3 -m venv venv
```

2. Activate the virtual environment:
```bash
source venv/bin/activate
```

3. Install the required packages
```bash
pip install -r requirements.txt
```

4. Build the project into a single binary file suitable for your OS:
```bash
python3 -m PyInstaller --onefile ./lpass.py
```

5. Once the compilation has finished, the binary file will be located at `./dist/lpass`
```bash
./dist/lpass
```

Bonus - If you want to do it all in one step:
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python3 -m PyInstaller --onefile ./lpass.py
./dist/lpass
```