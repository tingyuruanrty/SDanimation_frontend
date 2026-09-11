# SDanimation_frontend
# host:
npx vite

# plan ahead:
if i end up using video generation model instead of sdxl, i could replace the lora with style reference

# character object:
id/character_id(this is guaranteed to be unique, so that even two characters have the same name, won't lead to any problem)
name/display_name(it's character's name, will be display on the character choose modal)
trigger_word
lora_filename(filename on comfy cloud)

# Todo:
1. i need to fix the style for the preview section, the content is overflowing the grid box
2. the preview image for the lora is probaboly not showed
3. i nead a download button, bath download the generated picture
4. manage synchronize/asynchronize