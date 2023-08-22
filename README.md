# Automated-data-synchronization
import boto3


mysns =  boto3.client("sns")


def lw(x,y):
    # TODO implement
    mysns.publish(
        Message='criticl alert s3 file deleted',
        Subject='s3 object deleted',
          TopicArn='arn:aws:sns:ap-south-1:413249457651:ChangesINBucket'
          )
    
