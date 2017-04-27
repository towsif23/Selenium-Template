# Selenium-Template
Web automation template through Java programming!






import java.util.concurrent.TimeUnit;

import org.junit.rules.Timeout;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class Webauto {

public static WebDriver driver;
	
	
	public static void main(String[] args) throws InterruptedException {

//Set up the property for the chrome driver script to be used by setting up the directory path.		
System.setProperty("webdriver.chrome.driver", "C:\\Users\\owner\\Documents\\chromedriver.exe");

//This will use the chrome browser to perform web tasks.
driver=new ChromeDriver();		

//Go to the Yahoo website by using the get command from driver.
driver.get("https://www.yahoo.com");

//Type in the search box of yahoo by using the findelement of driver. 
driver.findElement(By.xpath("//*[@id='uh-search-box']")).sendKeys("Auto Web");

//Click on the search button to pop up the list by using the click method.
driver.findElement(By.xpath("//*[@id='uh-search-button']")).click();

//The class has run successfully.
System.out.println("Class script has run successfully !");


	}

}
