# mounika
package com.java.program;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.firefox.FirefoxDriver;
import org.openqa.selenium.support.ui.Select;

public class Seleniumtraining {
	
	public static void main(String[] args){
		// TODO Auto-generated method stub
		

	WebDriver driver= new FirefoxDriver();
	driver.manage().window().maximize();
	driver.get("https://in.edit.yahoo.com/registration");
	WebElement lan = driver.findElement(By.xpath(".//*[@id='country-lang']"));
	Select lan1=new Select(lan);
	lan1.selectByIndex(9);
	driver.findElement(By.xpath(".//*[@id='first-name']")).sendKeys("mounika");
	driver.findElement(By.xpath(".//*[@id='last-name']")).sendKeys("jammi");
	driver.findElement(By.xpath(".//*[@id='user-name']")).sendKeys("jammimounika");
	driver.findElement(By.xpath(".//*[@id='password']")).sendKeys("jammimounika123");
	driver.findElement(By.xpath(".//*[@id='mobile']")).sendKeys("9949485281");
	WebElement e=driver.findElement(By.xpath(".//*[@id='day']"));
	Select s=new Select(e);
	s.selectByValue("16");
	
			WebElement e1=driver.findElement(By.xpath(".//*[@id='month']"));
			Select s1=new Select(e1);
			s1.selectByValue("12");
			
			WebElement e2=driver.findElement(By.xpath(".//*[@id='year']"));
			Select s2=new Select(e2);
			s2.selectByValue("1993");
		driver.findElement(By.xpath(".//*[@id='gender-wrapper']/fieldset/div/label[2]")).click();
		driver.findElement(By.xpath(".//*[@id='mobile-rec']")).sendKeys("949485281");
		driver.findElement(By.xpath(".//*[@id='relationship']")).sendKeys("married");
		driver.findElement(By.xpath(".//*[@id='yui_3_7_3_8_1444625748754_5542']/input")).submit();
		
	}

	
	}



		
