Darienn López Plaza, darlopezp, IIT414W, 06-03-2026

Windows 11, Python 3.12.10, pip 25.0.1

# Setup Instructions

## Using `requirements.txt` (pip)

**Step 1.** Open a terminal (Command Prompt or PowerShell) and go to this folder:
```
cd path\to\iit414w-lab00-darlopezp
```

**Step 2.** Create a new virtual environment:
```
python -m venv venv
```

**Step 3.** Activate it:
```
venv\Scripts\activate
```
> You should see `(venv)` at the start of your prompt.

**Step 4.** Install all packages:
```
pip install -r requirements.txt
```

**Step 5.** Register the environment as a Jupyter kernel:
```
python -m ipykernel install --user --name iit414w --display-name "IIT414W"
```

**Step 6.** Open VS Code, open any `.ipynb` notebook, and select **IIT414W** as the kernel (top-right corner).


## Verify the setup

Run the first two cells of `setup_check.ipynb` top-to-bottom. If all packages print their versions without errors, the environment is ready.

Next, you can run all cells of both files.

# Problems encountered

When I say to AI to resolve an exercise, if I only write "resolve this", obtains results so basics. I can get better results when I explain more what I want and say "Explain me"-

Also, I had a problem with Jolpica API. The error was a bad URL because the AI changed this.

# Expected Outputs

If you follow these steps you can see a lot of tables and graphs about F1 and Agentic Engineer examples.
