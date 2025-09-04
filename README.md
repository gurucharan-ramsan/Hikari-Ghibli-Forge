# Hikari-Ghibli-Forge
Hikari Labs is an open-source tool that converts any video into a Studio Ghibli–inspired animation. Powered by AI, it processes each frame to recreate the warm, hand-painted look of classic Ghibli films. Simple to use, flexible, and perfect for anyone who wants to bring a little animation magic into their footage.

from diffusers import ControlNetModel, StableDiffusionXLControlNetImg2ImgPipeline, AutoencoderKL
from diffusers import DDIMScheduler, EulerAncestralDiscreteScheduler
from diffusers.utils import load_image
from pathlib import Path
from PIL import Image
import matplotlib.pyplot as plt
import torch
import numpy as np
import cv2
import os
from google.colab import files
from IPython.display import HTML
from base64 import b64encode
