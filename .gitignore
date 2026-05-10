import os
import shutil

def sort_files(folder):
    for filename in os.listdir(folder):
        path = os.path.join(folder, filename)
        if os.path.isfile(path):
            ext = os.path.splitext(filename)[1].lower()
            dest = os.path.join(folder, ext[1:] if ext else 'other')
            os.makedirs(dest, exist_ok=True)
            shutil.move(path, os.path.join(dest, filename))

if __name__ == "__main__":
    sort_files('/путь/к/загрузкам')
