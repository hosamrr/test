# test
tesy
استيراد  النظم
 وقت الاستيراد
 طلبات الاستيراد

__banner__  =  "" "
\ 033 [1 ؛ 33 م ____ __ _____ ____ \ 033 [1 ؛ 37 م
\ 033 [1 ؛ 33 م / __ / __ _ / / _____ / ___ / __ _ / / / \ 033 [1 ؛ 37 م
\ 033 [1 ؛ 33 م / _ // _ `/ '_ / -_) / / __ / _` / / /   \ 033 [1 ؛ 37 م
\ 033 [1 ؛ 33 م / _ /   \\ _ ، _ / _ / \\ _ \\ \\ __ /   \\ ___ / \\ _ ، _ / _ / _ /    \ 033 [1 ؛ 37 م
مصنوع من <3 Azis_riaz (azisek_)
""

def  البريد العشوائي ():
	الخيارات = sys . ارغف [ 1 ]
	الهاتف = sys . ارغف [ 2 ]
	إذا كان  النظام . argv [ 1 ] ==  "-c" :
		طباعة  __راية__
		param  = { 'msisdn' : '' + sys . argv [ 2 ]، 'Accept' : 'call' }
		العد  =  0
		بينما ( العد  <  3 ):
			ص  =  الطلبات . نشر ( 'https://www.tokocash.com/oauth/otp' ، البيانات = بارام )
			إذا كان  "otp_attempt_left"  في  r . نص :
				طباعة ( " \ 033 [1؛ 32m [OK] Sukses Dikirim ... Tunggu 60 Detik ... \ 033 [0m" )
			آخر :
				طباعة ( " \ 033 [1؛ 31m [FAILED] Gagal Dikirim: (... Tunggu 60 Detik ... \ 033 [0m" )
			الوقت . النوم ( 60 )
			العد  =  العد  +  1
		طباعة ( " \ 033 [1؛ 36m [تم] الخروج ..." )
		sys . مخرج ( 1 )
	آخر :
		طباعة  __راية__
		طباعة  "Usage: fakecall.py -c PHONE"
		طباعة  "fakecall.py: خطأ: يتطلب خيار٪ s وسيطة"  خيارات ٪
		sys . خروج ()

إذا  __name__  ==  '__main__' :
	إذا كان  len ( sys . argv ) ! =  3 :
		طباعة  __راية__
		طباعة  "Usage: fakecall.py -c PHONE"
		sys . خروج ( 0 )
	آخر :
		البريد العشوائي ()
