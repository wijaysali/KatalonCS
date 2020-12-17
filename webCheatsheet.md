### WebUI Basic 
'Buka Browser dan mengarahkan ke url demoAUT'
WebUI.openBrowser('')
  
  ----------

'Menutup Browser'
WebUI.closeBrowser()


### WebUI Accept Alert

'buka browser dan mengarahkan ke website dimana akan menampilkan Alert'
WebUI.openBrowser(GlobalVariable.G_SiteURL)

'Menerima Alert ketika Alert ditampilkan'
WebUI.acceptAlert()

'Menutup Browser'
WebUI.closeBrowser()


### WebUI Auth
'Buka Browser dan mengarahkan ke url yang mau ditest'
WebUI.openBrowser('')

'Isi Username dan Password di Dialog ( Form Input ) Auth'
WebUI.authenticate('http://the-internet.herokuapp.com/basic_auth', 'admin', 'admin', 12)

'Menutup Browser'
WebUI.closeBrowser()


### WebUI Back 
'Buka Browser dan mengarahkan ke url demo AUT'
WebUI.openBrowser('http://demoaut.katalon.com/')

'Klik pada Tombol Make Appointment'
WebUI.click(findTestObject('Page_CuraHomepage/btn_MakeAppointment'))

'Kembali ke halaman sebelumnya setelah mengarahkan ke halaman Make Appointment'
WebUI.back()

'Menutup Browser'
WebUI.closeBrowser()

### WebUI Check
digunakan untuk cek (check-box / radio-button)

'Buka Browser dan mengarahkan ke url demo AUT' 
WebUI.openBrowser('http://demoaut.katalon.com/')

'Klik pada Tombol Make Appointment'
WebUI.click(findTestObject('Page_CuraAppointment/btn_BookAppointment'))

' Pilih Checkbox yang value nya Medicaid"
WebUI.check(findTestObject('Page_CuraAppointment/chk_Medicaid'))

'Menutup Browser'
WebUI.closeBrowser()

