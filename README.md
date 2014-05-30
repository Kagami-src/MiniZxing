MiniZxing
=========
core code of Zxing for android

=========
Intent i=new Intent(Activity.this, CaptureActivity.class);
startActivityForResult(i, CaptureActivity.QR_RESULT);

=========

in your activity 

=========
@Override
protected void onActivityResult(int requestCode, int resuleCode, Intent i) {
	if(requestCode==CaptureActivity.QR_RESULT&&resuleCode==1){
		Log.d("kagami", i.getStringExtra("data"));
	}
	super.onActivityResult(requestCode, resuleCode, i);
}

=========
