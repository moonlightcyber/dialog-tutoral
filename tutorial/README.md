## Creating a modal with a ```<dialog>``` tag

For a long time the only way to create a modal on a webpage was a series of divs nested into eachother.
But recently browsers have started allowing the ```<dialog>``` tag.
This tag saves a bunch of time as now with Javascript you can call methods to open the dialog or close it, Cutting work time in half.

### Tutoral

#### Dialog

here is an example of what a form in a dialog tag looks like

```html
<!-- dialog with form -->
<dialog>
	<form method="dialog">
		<label>Name</label>
		<input type="text" name="name" />
		<button>Submit</button>
	</form>
</dialog>
```

#### Open dialog

```showModal()``` opens the modal

```html
<!-- dialog with form -->
<dialog id="modal-dialog">
	<form method="dialog">
		<label>Name</label>
		<input type="text" name="name" />
		<button>Submit</button>
	</form>
</dialog>
```

```javascript
document.querySelector("#modal-dialog").showModal()
```

#### Close dialog

```close()``` closes the modal

```javascript
document.querySelector("#modal-dialog").close()
```



### References
- [useful angle](https://usefulangle.com/post/110/html-dialog-element-to-create-modal-lightbox)