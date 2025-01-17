# ChatGPT Conversation Heatmap

This project visualizes daily ChatGPT activity as a GitHub-style contribution heatmap, showing the number of conversations per day.
![chatgpt-heatmap](https://raw.githubusercontent.com/raselmandol/chatgpt-heatmap/refs/heads/main/assets/1.png)


The original version of [ai-heatmap](https://github.com/chiphuyen/aie-book/blob/main/scripts/ai-heatmap.ipynb) is from author Chip Huyen([@chiphuyen](https://github.com/chiphuyen)) and the repo [aie-book](https://github.com/chiphuyen/aie-book) (every AI engineer building real-world applications should read this book).

- Converts exported ChatGPT conversation data into a heatmap.
- Displays activity counts by day, similar to GitHub contribution graphs.


## Prerequisites

Before you begin, ensure you have the following installed:

- `Python 3.8+`
- `matplotlib`
- `numpy`

## Exporting ChatGPT Data

1. Visit your ChatGPT account [settings](https://chatgpt.com/#settings).
2. Navigate to **Data Controls**.
3. Click **Export Data** and follow the instructions.
4. You will receive a `.zip` file in your email. Download and extract it.
5. Locate the `conversations.json` file from the extracted data.

## Exporting Claude Data

1. Visit your Claude account [settings](https://claude.ai/settings/account).
2. Click **Export Data** and follow the instructions.
3. You will receive a `.zip` file in your email. Download and extract it.
4. Locate the `conversations.json` file from the extracted data.


## Running the Heatmap

1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

2. Load the `chatgpt_heatmap.ipynb` file.
3. Update the `json_file_path` variable with the path to your `conversations.json` file:
   ```python
   json_file_path = "path_to_your_conversations.json"
   ```
4. Run all cells to generate the heatmap.


## Sample Heatmap

![Sample Heatmap](https://raw.githubusercontent.com/raselmandol/chatgpt-heatmap/refs/heads/main/assets/1.png)
![Sample Heatmap](https://raw.githubusercontent.com/raselmandol/chatgpt-heatmap/refs/heads/main/assets/2.png)


## Customization

- **Color Map**: Modify the `ListedColormap` in the script to adjust heatmap colors.
- **Borders**: Adjust `edgecolors` and `linewidths` in the `pcolormesh` function.

## Extra 

You can do the same for Claude, as both have the file named conversations.json.

