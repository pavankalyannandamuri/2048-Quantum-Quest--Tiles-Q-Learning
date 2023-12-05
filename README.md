# Quantum 2048 Quest Tiles - Q-Learning

## Project Structure

Here is an overview of the project structure:

- `agents`: Contains scripts for training and evaluating agents. This includes Q-learning implementations and necessary code for custom callbacks and policies.
- `docs`: Includes resources such as GIFs and other documentation.
- `hyperparams`: Contains YAML files detailing hyperparameters for agents.
- `models`: Holds pretrained agents.
- `utils`: Contains auxiliary scripts for plotting results.

## Installation

It is recommended to use a separate Python 3.7 environment for this project due to compatibility issues when loading models created using Python 3.7 on other versions. The dependencies include PyYAML, OpenAI Gym, TensorFlow 1.15.x, Stable Baselines, and gym-text2048. Install them using:

```bash
pip install -r requirements.txt
```

Install the gym-text2048 environment:

```bash
git clone https://github.com/mmcenta/gym-text2048
pip install -e gym-text2048
```

## Running

### Interactive Player for Humans:

```bash
python agents/play.py
```

### Random Agent:

```bash
python agents/random_agent.py
```

### Q-Learning:

#### To Show an Agent Reaching 2048:

```bash
python agents/q_learning.py --r2048
```

#### To Demo Pretrained Models:

```bash
python agents/q_learning.py -mn MODEL_NAME --demo
```

##### Example:

```bash
python agents/q_learning.py -mn q_agent_v1 --demo
```

#### To Train:

```bash
python agents/q_learning.py -mn MODEL_NAME --train
```

#### To Evaluate:

```bash
python agents/q_learning.py -mn MODEL_NAME --eval
```

#### Complete Usage:

```bash
python agents/q_learning.py -h
```

## Plotting Training Logs:

### To Plot All Training Logs:

```bash
python utils/plot_log_multi.py
```

### To Plot a Specific Training Log:

```bash
python utils/plot_log.py PATH_TO_LOG
```

#### Example:

```bash
python utils/plot_log.py logs/q_agent_v1.npz
```
"# 2048-Quantum-Quest-Tiles-Q-Learning" 
