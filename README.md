< < < < < < < .Mine
<? php
/ * LOGIN FACEBOOK + LOGOUT - PHP SDK V4.0
 * file - index.php
 * Pengembang - Krishna Teja GS
 * Situs web - http://packetcode.com/apps/fblogin-basic/
 * Tanggal - 27 September 2014
 * lisensi - Lisensi Publik Umum GNU ver
si 2 atau yang lebih baru
* /

/ * PENCANTUMAN FILE PERPUSTAKAAN * /
	membutuhkan_once ( 'lib / Facebook / FacebookSession.php' );
	membutuhkan_once ( 'lib / Facebook / FacebookRequest.php' );
	membutuhkan_once ( 'lib / Facebook / FacebookResponse.php' );
	memerlukan_once ( 'lib / Facebook / FacebookSDKException.php' );
	memerlukan_once ( 'lib / Facebook / FacebookRequestException.php' );
	membutuhkan_once ( 'lib / Facebook / FacebookRedirectLoginHelper.php' );
	memerlukan_once ( 'lib / Facebook / FacebookAuthorizationException.php' );
	membutuhkan_once ( 'lib / Facebook / GraphObject.php' );
	membutuhkan_once ( 'lib / Facebook / GraphUser.php' );
	membutuhkan_once ( 'lib / Facebook / GraphSessionInfo.php' );
	membutuhkan_once ( 'lib / Facebook / Entities / AccessToken.php' );
	memerlukan_once ( 'lib / Facebook / HttpClients / FacebookCurl.php' );
	memerlukan_once ( 'lib / Facebook / HttpClients / FacebookHttpable.php' );
	memerlukan_once ( 'lib / Facebook / HttpClients / FacebookCurlHttpClient.php' );

/ * GUNAKAN NAMESPACES * /
	
	gunakan  Facebook \ FacebookSession ;
	gunakan  Facebook \ FacebookRedirectLoginHelper ;
	gunakan  Facebook \ FacebookRequest ;
	gunakan  Facebook \ FacebookResponse ;
	gunakan  Facebook \ FacebookSDKException ;
	gunakan  Facebook \ FacebookRequestException ;
	gunakan  Facebook \ FacebookAuthorizationException ;
	gunakan  Facebook \ GraphObject ;
	gunakan  Facebook \ GraphUser ;
	gunakan  Facebook \ GraphSessionInfo ;
	gunakan  Facebook \ FacebookHttpable ;
	gunakan  Facebook \ FacebookCurlHttpClient ;
	gunakan  Facebook \ FacebookCurl ;

/*PROSES*/
	
	//1. Sesi Statistik
	 session_start ();

	// periksa apakah pengguna ingin keluar
	 if ( isset ( $ _REQUEST [ 'logout' ])) {
	 	belum disetel ( $ _SESSION [ 'fb_token' ]);
	 }
	
	//2. Gunakan id aplikasi, rahasia, dan url pengalihan 
	$ app_id = '869447339769084' ;
	$ app_secret = '637cddd0a52beccdc0b5d549927a9dbb' ;
	$ redirect_url = 'http://kiandastream.globusapps.com/apps/login' ;

	//3. Inisialisasi aplikasi, buat objek pembantu dan dapatkan fb sess
	 FacebookSession :: setDefaultApplication ( $ app_id , $ app_secret );
	 $ session = new  FacebookSession ( 'access-token-here' );

// Dapatkan objek GraphUser untuk pengguna saat ini:

coba {
  $ me = ( FacebookRequest baru  (
    $ sesi , 'GET' , '/ me'
  )) -> eksekusi () -> getGraphObject ( GraphUser :: className ());
  echo  $ saya -> getName ();
} tangkap ( FacebookRequestException  $ e ) {
  // Graph API mengembalikan kesalahan
} catch (\ Exception  $ e ) {
  // Terjadi kesalahan lain
}










	
=======
<? php
/ * LOGIN FACEBOOK + LOGOUT - PHP SDK V4.0
 * file - index.php
 * Pengembang - Krishna Teja GS
 * Situs web - http://packetcode.com/apps/fblogin-basic/
 * Tanggal - 27 September 2014
 * lisensi - Lisensi Publik Umum GNU versi 2 atau yang lebih baru
* /

/ * PENCANTUMAN FILE PERPUSTAKAAN * /
	membutuhkan_once ( 'lib / Facebook / FacebookSession.php' );
	membutuhkan_once ( 'lib / Facebook / FacebookRequest.php' );
	membutuhkan_once ( 'lib / Facebook / FacebookResponse.php' );
	memerlukan_once ( 'lib / Facebook / FacebookSDKException.php' );
	memerlukan_once ( 'lib / Facebook / FacebookRequestException.php' );
	membutuhkan_once ( 'lib / Facebook / FacebookRedirectLoginHelper.php' );
	memerlukan_once ( 'lib / Facebook / FacebookAuthorizationException.php' );
	membutuhkan_once ( 'lib / Facebook / GraphObject.php' );
	membutuhkan_once ( 'lib / Facebook / GraphUser.php' );
	membutuhkan_once ( 'lib / Facebook / GraphSessionInfo.php' );
	membutuhkan_once ( 'lib / Facebook / Entities / AccessToken.php' );
	memerlukan_once ( 'lib / Facebook / HttpClients / FacebookCurl.php' );
	memerlukan_once ( 'lib / Facebook / HttpClients / FacebookHttpable.php' );
	memerlukan_once ( 'lib / Facebook / HttpClients / FacebookCurlHttpClient.php' );

/ * GUNAKAN NAMESPACES * /
	
	gunakan  Facebook \ FacebookSession ;
	gunakan  Facebook \ FacebookRedirectLoginHelper ;
	gunakan  Facebook \ FacebookRequest ;
	gunakan  Facebook \ FacebookResponse ;
	gunakan  Facebook \ FacebookSDKException ;
	gunakan  Facebook \ FacebookRequestException ;
	gunakan  Facebook \ FacebookAuthorizationException ;
	gunakan  Facebook \ GraphObject ;
	gunakan  Facebook \ GraphUser ;
	gunakan  Facebook \ GraphSessionInfo ;
	gunakan  Facebook \ FacebookHttpable ;
	gunakan  Facebook \ FacebookCurlHttpClient ;
	gunakan  Facebook \ FacebookCurl ;

/*PROSES*/
	
	//1. Sesi Statistik
	 session_start ();

	// periksa apakah pengguna ingin keluar
	 if ( isset ( $ _REQUEST [ 'logout' ])) {
	 	belum disetel ( $ _SESSION [ 'fb_token' ]);
	 }
	
	//2. Gunakan id aplikasi, rahasia, dan url pengalihan 
	$ app_id = '305513519653069' ;
	$ app_secret = '7d15bdfc44197c88c765c44dfd2d7acf' ;
	$ redirect_url = 'http://kiandastream.com/apps/login/' ;

	//3. Inisialisasi aplikasi, buat objek pembantu dan dapatkan fb sess
	 FacebookSession :: setDefaultApplication ( $ app_id , $ app_secret );
	 $ session = new  FacebookSession ( 'access-token-here' );

// Dapatkan objek GraphUser untuk pengguna saat ini:

coba {
  $ me = ( FacebookRequest baru  (
    $ sesi , 'GET' , '/ me'
  )) -> eksekusi () -> getGraphObject ( GraphUser :: className ());
  echo  $ saya -> getName ();
} tangkap ( FacebookRequestException  $ e ) {
  // Graph API mengembalikan kesalahan
} catch (\ Exception  $ e ) {
  // Terjadi kesalahan lain
}










	
>>>>>>> . r3
