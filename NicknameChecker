import pyautogui
import time
import keyboard
import win32api, win32con


def click(x, y):
    win32api.SetCursorPos((x, y))
    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTDOWN, 0, 0)
    time.sleep(0.1)  # This pauses the script for 0.1 seconds
    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP, 0, 0)

filename = input('Enter wordlist name(with extension):')

file = open(filename)

content = file.readlines()
x = -1

print('\n8 sec to start')
time.sleep(8)


while True:
    x += 1
    click(286, 131)
    time.sleep(1.5)
    keyboard.press_and_release('backspace')
    time.sleep(0.1)
    keyboard.press_and_release('backspace')
    time.sleep(0.1)
    keyboard.press_and_release('backspace')
    time.sleep(0.1)
    keyboard.press_and_release('backspace')
    time.sleep(0.1)
    keyboard.press_and_release('backspace')
    time.sleep(0.1)
    keyboard.press_and_release('backspace')
    time.sleep(0.1)
    keyboard.press_and_release('backspace')
    time.sleep(0.5)
    keyboard.write(content[x])
    time.sleep(1)
    click(1180, 130)
    time.sleep(4)
    if pyautogui.pixel(620, 327)[2] == 255:
        print('Busy ' + content[x])
    else:
        print('Empty ' + content[x])
