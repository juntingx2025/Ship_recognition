Multi-modal, Multi-granularity Ship target recognition

## Models

* AISTransformer.py: AISTransformer.py is used to extract path features.
* RadoreTransformer.py: ImageTransformer.py is used to extract image features.
* main.py: main.py is used to integrate the entire model pipeline.
* PositionalEncoding.py: Positional encoding required for the transformer.
* GCN.py: Constructing the GCN model required for fusion.

## Usage

### Install dependencies

```python
pip install -r requirements.txt
```

### Obtain image embeddings

```python
python data/resnet50.py --file_path IMAGE_FOLDER_PATH
```

### Data process

```python
python data/data.py --task pretrain 
``

Complete Data Directory Structure


### Pretrain

```python
python main.py  --device cuda:0
```

## License

This project uses data from OpenStreetMap which is available under the Open Database License (ODbL). Any modifications to the data also adhere to this license. See [LICENSE](./LICENSE.txt) for more details.

