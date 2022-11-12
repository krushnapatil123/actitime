public class Test8 {

	public static void main(String[] args) throws InterruptedException{
		// TODO Auto-generated method stub
		System.setProperty("webdriver.chrome.driver", "./drivers/chromedriver.exe");
		ChromeDriver driver = new ChromeDriver();
		driver.get("https://demo.actitime.com/login.do");
		driver.get("https://www.facebook.com/");
		Navigation nav = driver.navigate();
		nav.back();
		Thread.sleep(2000);
		nav.forward();
		Thread.sleep(2000);
		nav.refresh();
	}
