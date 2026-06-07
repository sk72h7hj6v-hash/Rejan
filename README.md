# Rejan
Hi, I'm Rejan! I am a Data Science and Artificial Intelligence student based in Albania. I am passionate about turning raw data into actionable insights and exploring the security landscape through ethical hacking.

### 💻 My Favorite Snippet
Here is afunction I wrote to clean data in one of my projects:

```python
def clean_data(df):
    # Removes duplicates and handles missing values
    df = df.drop_duplicates()
    df.fillna(method='ffill', inplace=True)
    return df

    
    # 1. Standardize column names (lowercase and no spaces)
    df.columns = [col.lower().replace(' ', '_') for col in df.columns]
    
    # 2. Remove duplicates
    df = df.drop_duplicates()
    
    # 3. Handle missing values: Fill numerical with median, categorical with 'unknown'
    for col in df.select_dtypes(include=['number']).columns:
        df[col] = df[col].fillna(df[col].median())
        
    df.fillna('unknown', inplace=True)
    
    return df

# Example usage:
# cleaned_df = clean_dataset('raw_data.csv')



Tech Stack :
 Languages: Python (Pandas, NumPy, Matplotlib, PyTorch)
 
 Security: Kali Linux, Nmap, Network Security fundamentals
 
 Tools: Git, GitHub, SQL, Jupyter Notebooks, Terminal/Bash

 What I'm working on :
 Building a portfolio of data analysis and security-focused projects.
 Automating tasks and data workflows using Python.
 Participating in CTFs and learning to identify vulnerabilities in web applications.

Check out my portofolio:a link to my website -rejanisufi.uk
 
