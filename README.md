# ngx-file-viewer
    The file viewer component allow you to display various files in an angular project.
    File reader support:
    - [x] Images (PNG, JPEG...)
    - [ ] PDF
    - [ ] Markdown texts
    - [ ] CSV

    * [Install] (##Install)
    * [Setup] (##Setup)

## Disclaimer
    This is an experimental version.
    Please wait for v. 1.0.0
    I am only a young developper. So feel free to contribute on github.

## Install
   ```sh 
        $npm install --save ngx-file-viewer
   ``` 

## Setup
    Add `FileViewerComponent` to your application module.
    ```typescript
	import { FileViewerComponent } from 'ngx-file-viewer';

	@NgModule({
	    declarations: [
		AppComponent,
		FileViewerComponent
	    ],
	    imports: [
		...
	    ],
	    providers: [],
	    bootstrap: [AppComponent]
	})
	export class AppModule { }
    ```

    Then insert `file-viewer` in your page.
    ```typescript
        @Component({
            selector: 'app-root',
            templateUrl: `
                <file-viewer src='' width='' height='' controls=''></file-viewer>
            `
        })
    ```
## Usage

### Options
    * `src` : required - path to the file to display
    * `width` : required - width of the div
    * `height` : required - height of the div
    * `controls` : non-required - (true/false) By default false, show controls
