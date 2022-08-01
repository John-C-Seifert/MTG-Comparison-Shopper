# MTG-Comparison-Shopper
Goal: Input the Magic the Gathering Cards you want to buy. The program will compare which website has the least TOTAL price for the cards you input, and will then construct a cart from the cheapest website for the user. It will save the average magic the gathering player loads of money when buying decks with minimal effort.

THIS PROJECT IS CODED USING PYTHON

This project is still in the works. I am adding to the program component by component, so it is certaintly not finished. The purpose of this repository is just to keep track of my progress as I upload each component to this repository until I consider the program "finished". 

Base Plan(As of Start):
  Components 1 and 2: Will develop a program that can scrape cardkingdom, https://www.cardkingdom.com/, one of the main online Magic the Gathering Stores, for its cards and prices. Given a list of cards, this program should be able to return a total. Will do the same for star city games, https://starcitygames.com/, another one of the main Magic the Gatheirng Stores
  Components 3 and 4: Will develop a way to construct a cart for the user, on cardkingdom, so they don't have to input the cards twice, once in my program and once on the site. I will also do the same for Star City Games as well.
  Component 5: A program that will compare the prices of Star City Games and Cardkingdom to give the user the best option. Cardkingdom has some cards cheaper than those on Star City Games and vice versa. Maybe the cheapest option will be a mix of both sites, some from Star City and some from Cardkingdom. However, with shipping costs kicking in if some orders are below a certain amount, it might be hard to find the perfect balance between the two cites. I hope this compenent/program will be able to.
  Component 6: Create a user interface, so it is easy for the user to input cards and figure out how to use the program.
  
  
Additional Info

I use Beautiful Soup to scrape cardkingdom
I use Selenium to scape starcity because the website is dynamic, something I didn't know existed before this project
I also use Selenium to construct the cart for the user, so they don't have too

To learn Beautiful Soup, I would recommend watching these 4 videos in sequence
  1: https://www.youtube.com/watch?v=gRLHr664tXA
  2: https://www.youtube.com/watch?v=lOzyQgv71_4
  3: https://www.youtube.com/watch?v=lC6mucyD17k
  4: https://www.youtube.com/watch?v=zAEfWiC_KBU&t=574s
  After these, just play around with it. Find a website, and scrape it, see what happens
  If you have any questions, I would reccomend looking here for the answer, https://www.crummy.com/software/BeautifulSoup/bs4/doc/
  
 To learn Selenium, I recommend these tutorials
   https://www.youtube.com/playlist?list=PLzMcBGfZo4-n40rB1XaJ0ak1bemvlqumQ
   WARNING: These videos were made two years ago, and Selenium has changed since then which might create confusion. However, the concepts in the video remain the same. Just when you see him use statements like this, driver.find_element_by_id('main'), it won't work because the syntax has changed since then, which gave me a lot of trouble at first. So follow these steps instead. Also, this won't make sense until you watch the videos.
      Use these Import Statements:
            from selenium import webdriver
            from selenium.webdriver.common.by import By
            from selenium.webdriver.chrome.service import Service
       When constructing driver, do this instead.
          s = Service(r'C:\Program Files (x86)/chromedriver.exe')    // This is just the location of your chromedriver, it will vary for you. The video will explain
          driver = webdriver.Chrome(service=s)
       When using driver.find_element_by_id, use this instead
           driver.find_elements(By.ID, 'main')
        If you have any questions, I would recommend looking them up on stack overflow, I have found that to be helpful for selenium
 
For Those who Play Magic: I don't think I will be comparing TCG player prices, the biggest online magic retailer, in this project. TCG player is completely different from other online retailers because the cards don't come from one place; its just a ton of individual sellers competing with eachother. while TCG Player is generally the cheapest, customers who buy from TCG Player will often times recieve damaged cards or just not recieve them at all. Thats why many use Cardkingdom or Starcity Games. While more expensive, its easier to use and cards will come in pristine condition. MTG players who use TCG Player only use TCG player and have no need for a comparison shopper. However, MTG players who use cardkingdom may also use star city games or any other retailer whose cards come from one place, me being one the mtg players that uses cardkingdom or starcity.




 

