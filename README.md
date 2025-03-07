# todo


```csharp
 Bitmap bitmap = new Bitmap(@"C:\Work\image.jpg");
 Graphics graphics = Graphics.FromImage(bitmap);
 Brush brush = new SolidBrush(Color.FromKnownColor(KnownColor.Blue));
 Pen pen = new Pen(brush, 6);

// Add rectangle
 graphics.DrawRectangle(pen, 100, 100, 800, 600);


 string filenameNew = string.Format("{0}{1}{2}{3}{4}", Path.GetDirectoryName(filename), Path.DirectorySeparatorChar, "OD_", DateTime.Now.Ticks, ".jpg");
 bitmap.Save(filenameNew);
```
