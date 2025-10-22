## Behavior and 2p Calcium Imaging Analysis Code  
### for *Klinger, Wang et al.*, 2025  

*(Link will be added upon publication)*

---

### Instructions to Run the Code

#### 1. Download the Repository

**Folder structure:**
```
root
├── Analysis/               # Analysis code
├── GithubData/             # DF/F and behavior data
└── Master_pipeline.ipynb   # Master analysis notebook
```

---

#### 2. Preprocessing (Matlab)

1. Add the following folder to your MATLAB path:  
   ```
   ~/Analysis/behavior_process_matlab/
   ```

2. Open the script:  
   ```
   /Analysis/behavior_process_matlab/behavior_pipeline_full.m
   ```  

   Edit the first line to specify your own path:
   ```matlab
   root_path = '[your_own_path]/GithubData/Late_Learner';
   ```

3. Run the script to generate the processed behavior file.

4. Repeat the above step with:
   - `Early_Learner`
   - `Early_nonlearner`
   - `Late_nonlearner`

---

#### 3. Run the Master Pipeline

Open the following file in **Jupyter Notebook** to replicate the analysis from the paper:  
```
/Master_pipeline.ipynb
```

(see [README](./README.md) for additional details)