
About You.
-----------------
#  Introduce yourself.

    Thank you for giving me this opportunity.

    My name is Nikhil, and my qualification is Btech in computer science and I have 3+ years of experience as a software engineer in Php web development. i have been working as a software developer in a company here in kochi for last two years and recenlty resigned from there. My primary responsibility is to develop and enhance web applications in Php domain using frameworks sucj as Laravel/codeigniter etc
    
    As my current work experience and skills match your job requirements, I feel that I am a suitable candidate for this position.
 
## Describe your development environment. (Your OS, IDE, Editor and Config manager if any)

    Operating system familer with : Linux and Windows
    IDE: VS Code and Sublime Text
    Git 

## Social Profile
-------------------

    Your Github profile url :  https://github.com/nikhilmv
    LinkedIn profile : linkedin.com/in/nikhil
    -vasu-13412b235/
    Personal website, blog or something you want us to see. : Weblitz.in(technology related news, downloads etc built in laravel framework in 2020 currently under maintence )

 

## 1. Which all programming languages are installed on your system.

Php, react js

## 2.Write a function that takes a number and returns an array of its digits.

    <?php 
    function convertDigitToArray($number) {
        $digits = array();
        while ($number > 0) {
            $digit = $number % 10;
            array_unshift($digits, $digit);
            $number = floor($number / 10);
        }
        print_r($digits);
    } 
    convertDigitToArray(8418148); 
    ?>

## 3. Write function that translates a text to Pig Latin and back. English is translated to Pig Latin by taking the first letter of every word, moving it to the end of the word and adding ‘ay’. “Join with yellowfish” becomes “oinjay ithway ellowfishyay”.
 

    <?php 
    function translateToPigLatin($sentence) {
    
        $wordArray = explode(" ",$sentence);
    
        foreach ($wordArray as $key => $word) {
        $firstLetter = mb_substr($word, 0, 1);
        $wordArray[$key] = $wordArray[$key].$firstLetter;
        $wordArray[$key] = substr($wordArray[$key], 1);
        $wordArray[$key] = $wordArray[$key]."ay";
        echo  $wordArray[$key]." "; 
        }
    } 
    translateToPigLatin('Join with yellowfish'); 
    ?>



## 4. Write a function that rotates an array by k elements. For example [1,2,3,4,5,6] rotated by two becomes [3,4,5,6,1,2]. Try solving this without creating a copy of the array.


    <?php   
    
    function arrayRotate($arr) {
    $n = 2;  
    //Rotate the given array by n times toward left  
    for ($i = 0; $i < $n; $i++){   
        $first = $arr[0];  
        for($j = 0; $j < count($arr)-1; $j++){   
            $arr[$j] = $arr[$j+1];  
        }   
        $arr[$j] = $first;  
    }       
    print("Array after left rotation: <br>");  
        for ($i = 0; $i < count($arr); $i++) {   
            print($arr[$i] . " ");   
        }   
    }
    arrayRotate(array(1, 2, 3, 4, 5, 6)); 
    ?>  

## 5. Create a URL shortener using Laravel.

please find the given link for the repository

https://github.com/nikhilmv/URL-shortener