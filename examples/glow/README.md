# Glow using Skeltorch
How to run the example in your computer:

1. Clone Skeltorch in your computer:

```
git clone https://github.com/davidalvarezdlt/skeltorch.git
```

2. Change your current directory to the example:

```
cd skeltorch/examples/glow
```

3. Install dependencies using ``pip``:

```
pip install -r requirements.txt
```

4. Create a new experiment with your preferred name:

```
python -m glow --experiment-name my_experiment init --config-path config.default.json --config-schema-path config.schema.json
```

5. Run the train pipeline (set ``--device cuda`` to run on GPU):

```
python -m glow --experiment-name my_experiment train
```

6. (Optional) Run the test (set ``--device cuda`` to run on GPU):

```
python -m glow --experiment-name my_experiment test --epoch 10
```

7. (Optional) Visualize results using tensorboard:

```
tensorboard --logdir experiments/my_experiment
```