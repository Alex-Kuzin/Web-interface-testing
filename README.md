[![Build status](https://ci.appveyor.com/api/projects/status/f4tk1yuyr8i2p24c?svg=true)](https://ci.appveyor.com/project/Alex-Kuzin/web-interface)
/*package ru.netology;

import io.github.bonigarcia.wdm.WebDriverManager;
import org.junit.jupiter.api.AfterEach;
import org.junit.jupiter.api.BeforeAll;
import org.junit.jupiter.api.BeforeEach;
import org.junit.jupiter.api.Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.chrome.ChromeOptions;

import java.util.List;

import static org.junit.jupiter.api.Assertions.assertEquals;

class DebitCardApplication {
private WebDriver driver;

    @BeforeAll
    static void setUpAll() {
        WebDriverManager.chromedriver().setup();
    }

    @BeforeEach
    void setUp() {
        ChromeOptions options = new ChromeOptions();
        options.addArguments("--disable-dev-shm-usage");
        options.addArguments("--no-sandbox");
        options.addArguments("--headless");
        driver = new ChromeDriver(options);
        driver.get("http://localhost:9999");
    }

    @AfterEach
    void tearDown() {
        driver.quit();
        driver = null;
    }

    @Test
    void shouldTestV2() {
        driver.findElement(By.cssSelector("[data-test-id=`name`] input")).sendKeys("Василий Васильевич");
        driver.findElement(By.cssSelector("[data-test-id=`phone`] input")).sendKeys("+79270000000");
        driver.findElement(By.cssSelector("[data-test-id=`agreement`]")).click();
        driver.findElement(By.cssSelector("[button.button]")).click();
        String text = driver.findElement(By.className("data-test-id=`order-success`")).getText();
        var ActualText = driver.findElement(By.cssSelector("Ваша заявка успешно отправлена! Наш менеджер свяжется с вами в ближайшее время.")).getText().trim();
    }
}

plugins {
id 'java'
}

group 'ru.netology'
version '1.0-SNAPSHOT'

sourceCompatibility = 11

compileJava.options.encoding = "UTF-8"
compileTestJava.options.encoding = "UTF-8"

repositories {
mavenCentral()
}

dependencies {
testImplementation 'org.junit.jupiter:junit-jupiter:5.6.1'
testImplementation 'org.seleniumhq.selenium:selenium-java:4.8.3'
testImplementation 'io.github.bonigarcia:webdrivermanager:5.3.0'
}

test {
useJUnitPlatform()

}*/