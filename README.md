# Usage
Replace spaces with dashes, and prefix with uig-

eg: .uig-blu

Set direction with --uig-direction, set globally by putting it in html or body.

# Build Yourself

```location.href = 'https://uigradients.com';
e = document.querySelectorAll('.palette__gradient');
x = "html{--uig=direction: to right;}";
for(i = 0; i < e.length; i++){
	x += ".uig-"+e[i].firstChild.innerHTML.replace(/\s+/g, '-').toLowerCase()+"{background: "+e[i].style.background.replace('to right', 'var(--uig-direction)')+";}";
}```
