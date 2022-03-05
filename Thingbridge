package Azure;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.support.ui.Select;

public class LoginPage {

	public static void main(String[] args) throws InterruptedException {

		 //Invoke browser & open url 
		
		 System.setProperty("webdriver.chrome.driver", "D:\\New folder\\Chromedriver98\\chromedriver.exe");
	       WebDriver driver = new ChromeDriver ();
	       driver.manage().window().maximize();
	       driver.get("https://jt-dev.azurewebsites.net/#/SignUp");
	       
	       
	      //Validate Language
	     
	   System.out.println(driver.findElement(By.xpath("//*[@id=\"language\"]/div[1]/span/span[2]")).getText());
	driver.findElement(By.xpath("//*[@id=\"language\"]/div[1]/span/span[2]")).click();
	driver.findElement(By.xpath("//*[@id=\"ui-select-choices-row-1-1\"]/a/div")).click();
	System.out.println( driver.findElement(By.xpath("//*[@id=\"language\"]/div[1]/span/span[2]")).getText());
	
	// Fill the details
	
	driver.findElement(By.xpath("//*[@id=\"name\"]")).sendKeys("Aditya More");
	driver.findElement(By.xpath("//*[@id=\"orgName\"]")).sendKeys("Aditya");
	driver.findElement(By.xpath("//*[@id=\"singUpEmail\"]")).sendKeys("adityamore1818@gmail.com");
	driver.findElement(By.xpath("//*[@id=\"content\"]/div/div[3]/div/section/div[1]/form/fieldset/div[4]/label/span")).click();
	driver.findElement(By.xpath("//*[@id=\"content\"]/div/div[3]/div/section/div[1]/form/fieldset/div[5]/button")).click();
	
	Thread.sleep(5000);
	
	//Validate email sent message
	
	String message = driver.findElement(By.xpath("//*[@id=\"content\"]/div/div[3]/div/section/div[1]/form/div/span")).getText();
	System.out.println(message) ;
		}  
		
	       
	

}
