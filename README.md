# Using YoutubeFeeds

``` 
YoutubeFeeds.Youtube youtube = new YoutubeFeeds.Youtube();
var videos = youtube.getVideos("your channel id");
if (youtube.status)
{
   foreach(var video in videos){
      MessageBox.Show(video.Value.video_title); // video title
      MessageBox.Show(video.Value.video_description); // video description
      MessageBox.Show(video.Value.video_thumbnail); // video thumbnail
      MessageBox.Show(video.Value.video_url); // video url
   }
}else{
   MessageBox.Show(youtube.error_msg);
}
```
