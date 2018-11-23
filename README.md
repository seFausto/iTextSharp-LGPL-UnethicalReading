
### Install

` Install-Package iTextSharp-LGPL-Unetchical-Reading `

### Usage

```cs

    PdfReader.UnethicalReading = true;
    
    PdfReader reader = new PdfReader("protected-pdf-form.pdf");
    PdfStamper stamper = new PdfStamper(reader, File.Create("protected-pdf-form-out.pdf"));

    stamper.AcroFields.SetField("Field1", "Value1");
    stamper.Close();
    reader.Close();

 ```

