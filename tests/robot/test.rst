.. code:: robotframework

    *** Variables ***
    ${test} =    hello world

    *** Settings ***
    Documentation   test script for Variables

    *** Test Cases ***
    Hello Test Variables Case
        Log    ${test}    console=yes
        Hello Test Variables
        ${test} =     my world
        Log    ${test}    console=yes

    *** Keywords ***
    Hello Test Variables
        Log    hello world    console=yes