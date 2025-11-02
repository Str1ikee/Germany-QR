The code for revealing the flag:

import numpy as np
import matplotlib.pyplot as plt
from PIL import Image

# Încarcă imaginea (fișierul PNG)
img_path = r"distorted_qr.png"
img = Image.open(img_path)

# Transformă în array numpy
perturbation = np.array(img)

# Afișează imaginea
plt.imshow(perturbation)
plt.title("Distorted QR")
plt.axis("off")
plt.show()

# Informații despre imagine
print("Shape:", perturbation.shape)
print("Value range:", perturbation.min(), "to", perturbation.max())

The flag: SIGMOID_{cl4551c_cv_w1n5_S1gM014_N1C3_4N4Lys15_7r1ck5}
