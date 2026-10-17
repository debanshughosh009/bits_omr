# BITS Hyderabad 30Q OMR Checker

OMRChecker (MIT) bundled with the BITS 30-question sheet template.

## Run locally
python -m venv venv
.\venv\Scripts\Activate.ps1
pip install -r requirements.txt
pip install opencv-contrib-python
python main.py -i inputs\bits_omr

## Run with Docker
docker compose build
docker compose run --rm omr

Put scans in inputs/bits_omr/inputs/ (about 1791x2576 px). Results go to outputs/.
Expected for sample_273.jpg: Set=D, ID=2022A7PS2018H, q1-q10 = B B C D B C C D B B.