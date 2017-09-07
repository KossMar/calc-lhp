# calculator-lhp
//Calculator for LHP

//
//  main.m
//  CalculatorOC
//
//  Created by Mar Koss on 2017-09-06.
//  Copyright © 2017 Mar Koss. All rights reserved.
//

#import <Foundation/Foundation.h>

enum operation {
    add,
    subtract,
    multiply,
    divide
};

int main(int argc, const char * argv[]) {
    @autoreleasepool {
        
        float firstNumber = 24;
        float secondNumber = 578;
        float result;
        
        
        enum operation currentOperation = divide;
        
        switch (currentOperation)
        {
    case add:
        result = firstNumber + secondNumber;
            break;
    case subtract:
            result = firstNumber - secondNumber;
            break;
    case multiply:
            result = firstNumber * secondNumber;
            break;
    case divide:
            result = firstNumber / secondNumber;
            break;
        }
        
        NSLog(@"first number = %.4f\nsecond number = %.4f\nresult = %.4f", firstNumber, secondNumber, result);
           }
    return 0;
}
