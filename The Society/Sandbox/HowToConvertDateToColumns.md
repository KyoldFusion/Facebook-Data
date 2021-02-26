                                  --In order to convert your data into columns use this formula

p_pd = pd.read_csv('posts_and_comments.csv') #likes by me csv <br>
p_pd['Timestamp'] = pd.to_datetime(p_pd['Timestamp'],unit='s', yearfirst=True)  <br> 
p_pd['year'] = p_pd['Timestamp'].dt.year           <br> 
p_pd['month'] = p_pd['Timestamp'].dt.month         <br> 
p_pd['day'] = p_pd['Timestamp'].dt.day   <br> 
p_pd['hour'] = p_pd['Timestamp'].dt.hour   <br> 
p_pd.head()<br>

1. This code will convert the column first into a datetime format converted by seconds

2. The pd_pd['year'] creates a column off of the value of the TimeStamp column converted into year increments (/12) repeat the following and test with p_pd.head()

                                  --In order to convert your data into columns use this formula
                                  
  Copy & Paste this code into the likes_and_comments.csv to match you columns across code
        CommentTime,CommentTimeStamp,Comment,PostedBy,Action,Attachments,CommentGroup,CommentAttachments,AttachmentTimestamp,UploadIP,Title
        
  This will allow you to reuse the code
