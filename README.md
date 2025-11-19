from PIL import Image, ImageDraw, ImageFont

text = """Hyperkey Generator – Architecture Flowchart

START → Init Window → Build UI → Generate Password →
Show Output → Save to CSV → View History → Export → END
"""

# Create PNG canvas
img = Image.new("RGB", (1200, 800), (0, 0, 0))
draw = ImageDraw.Draw(img)

# Try loading a TTF font, fallback if missing
try:
    font = ImageFont.truetype("DejaVuSans.ttf", 32)
except:
    font = ImageFont.load_default()

# Draw text
draw.multiline_text((50, 50), text, fill=(255, 255, 255), font=font, spacing=20)

# Save PNG
path = "/mnt/data/Hyperkey_Flowchart.png"
img.save(path)

path
