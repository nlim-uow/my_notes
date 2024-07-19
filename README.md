# Converting colab outputs
``` python
import os
from google.colab import drive
drive.mount(drive_mount_point)
drive_mount_point = "/content/drive/"
file_name='Lab 4 '
file_path = os.path.join(drive_mount_point, "My Drive/Colab Notebooks/",file_name)
!jupyter nbconvert --to=html '{file_path}.ipynb'
!cp '{file_path}.html' /content/
```
