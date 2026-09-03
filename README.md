# SDanimation_frontend
# Todo:
1. i need to fix the style for the preview section

2. figure out how code worked

```javascript
if (!response.ok) throw new Error(`Server returned ${response.status}`);
    // result is a sequence of pictures, so return a json file include many picture link
	const result = await response.json();
					
	if (result.status === "good" && result.image_urls) {
  		// Grab all <i> slots inside .frame-grid
  		const frameSlots = document.querySelectorAll('.frame-grid i');

  		result.image_urls.forEach((url, index) => {
    		// Ensure the slot exists to prevent index-out-of-bounds errors
    		if (frameSlots[index]) {
    		frameSlots[index].innerHTML = `<img src="${url}" alt="Frame ${index + 1}" />`;
    		}
  		});
	}

```
