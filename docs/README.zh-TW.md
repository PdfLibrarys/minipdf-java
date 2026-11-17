# MiniPdf for Java

[Full guide (English)](../README.md)

## Quick start

[Maven Central artifact](https://central.sonatype.com/artifact/io.github.mini-software/minipdf)

```java
import io.github.minisoftware.minipdf.MiniPdf;
import java.nio.file.Files;
import java.nio.file.Paths;

try {
	MiniPdf.registerFont(
			"Noto Sans",
			Files.readAllBytes(Paths.get("fonts/NotoSans-Regular.ttf")));
	MiniPdf.convertToPdf(Paths.get("report.docx"), Paths.get("report.pdf"));
} finally {
	MiniPdf.clearRegisteredFonts();
}
```

使用方式請參閱 [Java 指南](../README.md)。

## Visual results

- [XLSX](https://mini-software.github.io/minipdf-web-page/?language=java&suite=issue&format=xlsx)
- [DOCX](https://mini-software.github.io/minipdf-web-page/?language=java&suite=issue&format=docx)

## License

[Apache License 2.0](../LICENSE).
