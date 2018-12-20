# Usage
Replace spaces with dashes, and prefix with uig-

eg: .uig-blu

# Build Yourself

```location.href = 'https://uigradients.com';
e = document.querySelectorAll('.palette__gradient');
x = "";
for(i = 0; i < e.length; i++){
	x += ".uig-"+e[i].firstChild.innerHTML.replace(/\s+/g, '-').toLowerCase()+"{background: "+e[i].style.background+";}";
}```
