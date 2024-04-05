# QRCode-project-
//It is simple qrcode
<br>
import qrcode as qr<br>
img = qr.make("https://www.youtube.com/")<br>
img.save("youtube.png" )<br>

<br>

//It is advance QRCode
<br>

import qrcode<br>
from PIL import Image<br>

qr = qrcode.QRCode(version = 1,<br>
                   error_correction = qrcode.constants.ERROR_CORRECT_H,<br>
                   box_size = 10,border=4,)<br>
qr.add_data("https://www.youtube.com/")<br>
qr.make(fit = True)<br>
img = qr.make_image(fill_color = "red",back_color= "blue")<br>
img.save("YOUTUBE.png")<br>


