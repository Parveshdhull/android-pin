# android-pin - Easily create multiple PIN views 

A simple JAVA class that can create multiple PIN views in a layout and auto executes code on entering PIN
![pin](https://user-images.githubusercontent.com/17097240/117448836-daf0d380-af5c-11eb-8c19-4359b48df928.gif)


## Prerequisite
1. Copy files from res folder to your specific folders in your project
2. In your XML file, create a LinearLayout or RelativeLayout where you want to insert PIN view and keep note of the ID

## Usage
### 1. Creating PIN

```
PINClass pinClass = new PINClass(this, R.id.linear_layout_insert_id, new Callable() {
	@Override
	public Object call() {
		submitPIN();
		return null;
	}
});
```
** NOTE:** You can keep the last argument as null, if you don't want any code to be auto executed

### 2. Other Functions

- `pinClass.getText();`
- `pinClass.clearPin();`
- `pinClass.getFocus();`

## Credits
This project is based on Tonia Tkachuk's [Blog](http://lomza.totem-soft.com/pin-input-view-in-android/)


## Websites
https://github.com/Parveshdhull
<br />https://twitter.com/ParveshMonu
<br />https://youtube.com/right2trick
