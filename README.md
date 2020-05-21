# TAO: A Large-Scale Benchmark for Tracking Any Object

[[Pre-print]()] [[Website](http://taodataset.org)]

[Achal Dave](http://www.achaldave.com/), [Tarasha Khurana](http://www.cs.cmu.edu/~tkhurana/), [Pavel Tokmakov](https://pvtokmakov.github.io/home/), [Cordelia Schmid](https://thoth.inrialpes.fr/~schmid/), [Deva Ramanan](http://www.cs.cmu.edu/~deva/)

## Setup

1. Clone this repo
    ```
    git clone https://github.com/achalddave/tao
    ```
1. Install TAO toolkit:
    ```
    pip install -e .
    ```

## Download dataset

TAO contains videos from 7 datasets: ArgoVerse, AVA, BDD-100k, Charades, HACS,
LaSOT, and YFCC-100M.
Where possible, we share the videos from these datasets, and provide scripts to
convert them to frames.
For ArgoVerse and LaSOT, the original datasets are shared as JPEG frames, so we
share those directly.
For HACS and AVA, we share a script to download the data directly from YouTube
and CVDF, respectively.

1. Download videos or frames for each source dataset:

    |           | Train | Val | Test |
    |-----------|-------|-----|------|
    | Charades  | [videos](https://drive.google.com/open?id=12dCphuV-ByVvktkuYFjYl_ZJ1ZVonBjy) | [videos](https://drive.google.com/open?id=1cjrxbf-wA8fxJ2AiHZeLmACZrqF4uPKb) | Coming soon |
    | BDD-100K  | [videos](https://drive.google.com/open?id=191QRs4O11EKHnDoscWws2g8BPiT35yZC) | [videos](https://drive.google.com/open?id=1zpoYCSU4SxIu35tZ1QpfZPpYMu8Kz2o2) | Coming soon |
    | YFCC-100M | [videos](https://drive.google.com/open?id=1j6hdIIFIBwRUthe2kozdB5QvcoBL_-eS) | [videos](https://drive.google.com/open?id=1Eh81fksBo5YwslblsRYib6-Dmy0KfF2k) | Coming soon |
    | LaSOT     | [frames](https://drive.google.com/open?id=1L0UUX_H7X1GGNt28v9I-g7UYRU1fHpaR) | [frames](https://drive.google.com/open?id=1UjLW_-0V3niEIyWhKJv0tSxzPaKr8264) | Coming soon |
    | ArgoVerse | [frames](https://drive.google.com/open?id=1jVhCHmaeFXJ6Vzbcn4LR_HqkVvTa2YHN) | [frames](https://drive.google.com/open?id=1iUyNg0XuruCizvcoiYyEUioK6_gThmqv) | Coming soon |

1. Uncompress each file in a single directory, which we will refer to as
   `$TAO_DIR`. This should have the following structure:

    ```
    ├── frames
    │  └── train
    │     ├── ArgoVerse
    │     └── LaSOT
    └── videos
        └── train
            ├── BDD
            ├── Charades
            └── YFCC100M
    ```
